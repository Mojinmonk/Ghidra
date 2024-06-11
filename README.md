# Ghidra
Github repository for Ghidra script developed for CS 413 Reverse Malware Analysis class

#ReportToFile.py

##Warning
There wasn't as much time as I would have liked to try and fine tune this, so there may be bugs in any of the methods that may call false positives or miss important details

---

## Usage
$ analyzeHeadless <PROJECT_PATH> <PROJECT_NAME> -inport <TARGET_FILENAME> -postScript <SCRIPT_FILENAME> <OUTPUT_FILENAME>

## Usage Breakdown
<PROJECT_PATH>
The path where your project will be stored, be sure to have this folder created before running the command.

<PROJECT_NAME>
The name you will give this project, can be different than the path, but is often named the same as the folder.

-import <TARGET_FILENAME>
The target_filename will include the full path to the file plus the file extension.

-postScript <SCRIPT_FILENAME>
If you stored your script in the ghidra_scripts or one of the other default directories you won't need to include the path to the script just the full name in cluding the file extension.

<OUTPUT_FILENAME>
This would include the full to the file location and project name you would like the result files saved as but not the extension as the script will append bits to the end.

## Usage Example
./analyzeHeadless /home/kali/headlessTest headlessTest -import /home/kali/Downloads/Week8a2.bin -postScript scriptTest.py /home/kali/headlessTest/output
