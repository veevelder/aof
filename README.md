## Android Obfuscation Fingerprinter

A *nix tool that is able to identifiy obfuscation methods in a given Android application. It will compare the identifiable obfuscation methods to form a fingerprint and determine the likelyhood it was obfuscated with either of the following Android obfuscators:

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
