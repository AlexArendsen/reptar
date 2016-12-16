# RepTAR
Simple CLI Frontend for extracting, viewing, and creating archive files.

## Synopsis

RepTAR is a simple, easy-to-use frontend for extracting, viewing, and creating
archive files. Support is provided for plain tar archives, as well as those
compressed using gzip, bzip2, xz, lzip, lzop, lzma, and compress. Plain zip and
rar archives are supported as well. File extensions are interpreted
automatically, eliminating the need to remember any pesky compression options
or flags!

## Usage

    reptar [MODE] [ARCHIVE] [FILES ...]

## Modes

RepTAR accepts the following commands:

* **extract**: Extracts the contents of an archive, according to its file
  extension.
* **view**: Prints the file listing contained by the archive without
  extraction.
* **create**: Creates an archive containing the specified `FILES`. The format
  is interpreted based on the archive's file extension.
* **help**: Prints a help message and quits.


## Examples

### Extract an archive

    reptar extract myarchive.tar.gz

### View an archive's contents

    reptar view myarchive.tar.bz2

### Create an archive

    reptar create myarchive.tgz file1.txt file2.bin file3.foo ...
