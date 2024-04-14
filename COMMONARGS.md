# Common arguments used for ExifTool
## Useful links
- [ExifTool options overview](https://exiftool.org/exiftool_pod.html#Option-Overview)
- [ExifTool file examples](https://exiftool.org/filename.html)
- [ExifTool examples](https://exiftool.org/examples.html)
- [ExifTool tag names](https://exiftool.org/TagNames/)
- [ExifTool library description](https://exiftool.org/ExifTool.html)

## Used arguments
```
# Enable LargeFileSupport API for parsing large media files.
-api
LargeFileSupport=1

# Allow duplicate tag names to be extracted.
-duplicates

# Extract values of unknown tags as well as unknown information 
# from some binary data blocks. This is the same as two '-u' options.
-unknown2

# Ignore minor errors and warnings. This enables writing to files 
# with minor errors and disables some validation checks which could result in minor warnings. 
-ignoreMinorErrors

# Show the progress when processing files. Implies the '-v0' option.
-progress

# Show the progress on console title aswell.
-progress:ExifTool %p%%
```