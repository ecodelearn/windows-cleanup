# windows-cleanup
3 simple commands that solve some troubles 



1. Type CDM in the search box. Do not hit enter.

2. select Run as Administrator then hit enter.

```plain text
DISM.exe /Online /Cleanup-image /Restorehealth" and hit enter.
sfc /scannow
DISM /Online /Cleanup-Image /StartComponentCleanup
```
