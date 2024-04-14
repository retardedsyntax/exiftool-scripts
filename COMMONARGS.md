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

# Overwrite the original FILE (instead of preserving it by adding _original to the file name) 
# when writing information to an image. Caution: This option should only be used if you already 
# have separate backup copies of your image files. The overwrite is implemented by renaming a 
# temporary file to replace the original. This deletes the original file and replaces it with 
# the edited version in a single operation. When combined with -o, this option causes the original
# file to be deleted if the output file was successfully written (ie. the file is moved instead of copied).
# If you wish to copy the files instead of overwriting them, see example 5 at 
# https://exiftool.org/filename.html about using the '-o' option.
-overwrite_original

# Preserve the filesystem modification date/time (FileModifyDate) of the original file 
# when writing. Note that some filesystems store a creation date (ie. FileCreateDate 
# on Windows and Mac systems) which is not affected by this option. This option is 
# superseded by any value written to the FileModifyDate tag.
-preserve

# Recurse all subdirectories.
-r
```