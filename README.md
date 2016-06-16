## Android Obfuscation Fingerprinter

Android Obfuscation Fingerprinter (aof) is a *nix tool that was written in Python, that is able to identifiy several obfuscation methods in any given Android application. The following is what obfuscation methods aof looks for:

* Source File IDX Obfuscation
* Removal of the BuildConfig Class
* Removal of Annotations
* Removal of Debug Information
* Class Name Obfuscation
* Variable Name Obfuscation
* Removal of Postions and Locals
* String Encryption

It will compare the identifiable obfuscation methods to form a fingerprint and determine the likelyhood it was obfuscated with either of the following Android obfuscators:

* Proguard
* Java Archive Grinder
* Zelix KlassMaster
* Allatori

## Usage
```
aof [OPTION]... FILENAME

Mandatory arguments for the OPTION field
  -a, --allatori              checks for Allatori obfuscation
  -A, --all                   checks against all obfuscators
  -h, --help                  prints this help message
  -j, --jarg                  checks for jarg (Java Archive Grinder) obfuscation
  -k, --klassmaster           checks for Zelix KlassMaster obfuscation
  -p, --proguard              checks for Proguard obfuscation
  -V, --verbose               prints what obfuscation was discovered
```
