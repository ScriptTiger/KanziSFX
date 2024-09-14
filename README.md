[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://docs.google.com/forms/d/e/1FAIpQLSfBEe5B_zo69OBk19l3hzvBmz3cOV6ol1ufjh0ER1q3-xd2Rg/viewform)

# KanziSFX: Kanzi SelF-eXtracting archive
KanziSFX is a minimal Kanzi decompressor to decompress an embedded Kanzi archive.

Usage: `kanzisfx [options...]`
Argument                  | Description
--------------------------|-----------------------------------------------------------------------------------------------------
 `-knz`                   | Output original Kanzi archive
 `-o <file>`              | Destination file
 `-info`                  | Show Kanzi bit stream info

`-` can be used in place of `<file>` to designate standard output as the destination.

Without any arguments, the embedded Kanzi stream will be decompressed into the working directory to a file of the same name as the executable, except with the `.exe` or `.app` extension removed. So, command-line usage is only optional and the end user can just execute the application as they would any other application for this default behavior.

# Appending a Kanzi archive to a KanziSFX executable
Download the latest pre-built release for the intended target system:  
https://github.com/ScriptTiger/KanziSFX/releases/latest

For appending a Kanzi archive to a KanziSFX executable, issue one of the following commands.

For Windows:
```
copy /b "KanziSFX.exe"+"file.knz" "MyKanziSFX.exe"
```

For Linux and Mac:
```
cat "KanziSFX" "file.knz" > "MyKanziSFX"
```

# More About ScriptTiger

For more ScriptTiger scripts and goodies, check out ScriptTiger's GitHub Pages website:  
https://scripttiger.github.io/

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=MZ4FH4G5XHGZ4)
