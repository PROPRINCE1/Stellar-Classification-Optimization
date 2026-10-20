# Possible Imputationable Columns
> obj_ID 'Reason: Object Identifier, the unique value that identifies the object in the image catalog used by the CAS'
> spec_obj_ID 'Reason: Unique ID used for optical spectroscopic objects (this means that 2 different observations with the same spec_obj_ID must share the output class) **There are no duplicates**'
> run_ID 'Reason: Run Number used to identify the specific scan'
> rerun_id 'Reason: Has only one value for everything'

## Right Skewed Columns
> 'alpha', 'delta'

## Left Skewed Columns
> 'u', 'g', 'r', 'z'

## Heavy Outliers in the following:
> 'g', 'z'

## One-Hot Encoding:
> The column 'class' contains the following three strings:
> 'GALAXY', 'STAR', 'QSO'
> They may be encoded as 100, 010, 001 respectively.

## Outlier Handling
> u,g,z had -9999 which was replaced by a nan during EDA
> Obersvation: mean < median in these columns (u,g,z,r,i) therefore later imputation may use median 