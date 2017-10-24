# msusel-quality-models
This repository is designated to contain the base quality models either designed or used by MSUSEL members/projects.

# Special Installation/Configuration/Run Notes:
### tools/QuamocoQualityModelEditor
This repository verion control only tracks the .qm files that are made using the Quamoco Quality Model Editor (QQME). The QQME application needs to be installed outside of this repository directory, with a reference link made to the .qm files in this repository as follows:
1. ~Download the QQME from (put link here)~ (todo: need to host QQME .zip file somewhere online)
2. Extract the .zip into a directory outside of this repository directory. This directory will be referred to as %LOCAL%
3. Open the QQME by double clicking `%LOCAL%\eclipse\eclipse.exe`
4. Within the QQME application, expand the `Basemodel` folder in the Project Explorer (lefthand side)
5. Delete the 4 exisiting default .qm files. (There might be two test-result files as well. If so, delete those too).
6. Create a link to the source controlled security model files in this repository as follows:
    1. Ensure this reposity has been locally cloned. The root directory of this repostiroy will be referred to as `~`.
    2. Select the .qm files found in `~/Basemodel/*.qm`
    3. Drag the .qm files to the `Basemodel` folder in the QQME.
    4. A `File Operation` dialog will appear. Select `Link to files` with link locations relative to `PROJECT_LOC`.
