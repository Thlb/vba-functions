# vba-functions

Some vba functions...

## Scripts

### export-vba-components.bas.vb : export all 

Export all vba components in external files in order to be able to git them

How does it work :
1. Export all vba components in temporary folder (pathTmp)
2. Compare each files exported in temporary folder (pathTmp) with the files exported previously (path)
  * if file in pathTemp = path --> no modification in the module since last export --> no action
  * if file in pathTemp != path --> module modified --> old version of module in "path" is replaced by new version of "pathTmp"
