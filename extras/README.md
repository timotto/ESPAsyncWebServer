### Extras
Additions to facilitate code modifications (for MS Win, similar can be done on Linux)

- **ehg.c (ehg.exe):** Tool to generate C-code array from file' bytes
Based on [bin2array](https://github.com/TheLivingOne/bin2array/)  PROGMEM keyword can optionally be added.

- **rehg.c (rehg.exe):** Tool to reverse C-code array generated by **ehg.exe** back to a file
Based on [c2bin](https://github.com/birkett/cbintools/tree/master/c2bin) 
First 4 lines of source are ignored, then parses the 0xHH - formated bytes 
until a } is found on separate new line.

### Tools
- [TCC : Tiny C Compiler](https://bellard.org/tcc/)  for **ehg** and  **rehg**  compiling on MS Win
- [7-Zip](https://www.7-zip.org)  Install 7z and use the included gzip as command line tool
- [Node.js](https://nodejs.org) Install Node with default settings, then run:

 ``` npm install html-minifier-terser -g,  npm install -g github-files-fetcher ```

### Batch files provided
- **do.bat:** Generates **edit.htm.gz.h** file
- **undo.bat:** Reverts **edit.htm** from C array header to file (still minified!)
- **update_ace.bat:** Updates **acefull.js.gz** file from latest GitHub Ace sources