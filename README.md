# Stellar-Classification-Optimization
How much can the number of astronomical observations be reduced while maintaining accurate classification of stars, galaxies, and quasars using machine learning?

# Initial Dataset Details *Before EDA*
1. obj_ID = Object Identifier, the unique value that identifies the object in the image catalog used by the CAS

2. alpha = Right Ascension angle (at J2000 epoch)
3. delta = Declination angle (at J2000 epoch)

4. u = Ultraviolet filter in the photometric system
5. g = Green filter in the photometric system
6. r = Red filter in the photometric system
7. i = Near Infrared filter in the photometric system
8. z = Infrared filter in the photometric system
9. redshift = redshift value based on the increase in wavelength

10. run_ID = Run Number used to identify the specific scan (Field Number assigned to a specific, small rectangular patch of the sky during an astronomical imaging scan)
11. rereun_ID = Rerun Number to specify how the image was processed

12. cam_col = Camera column to identify the scanline within the run (Also contains the information of location)
13. field_ID = Field number to identify each field (Patch of sky)

14. spec_obj_ID = Unique ID used for optical spectroscopic objects (this means that 2 different observations with the same spec_obj_ID must share the output class) 

15. class = object class (galaxy, star or quasar object)

16. plate = plate ID, identifies each plate in SDSS
17. MJD = Modified Julian Date, used to indicate when a given piece of SDSS data was taken
18. fiber_ID = fiber ID that identifies the fiber that pointed the light at the focal plane in each observation