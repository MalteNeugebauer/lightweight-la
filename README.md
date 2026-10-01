# Lightweight LA

This repository offers material to integrate Learning Analytics (LA) into web-based Learning Management Systems (LMS), esp. Moodle, lightweightly. I.e., they can be implemented by lecturers in their courses using the on-board tools of the LMS. Neither plugin installations nor additional technical permissions are required.

## Implementation

### Console-based - quick
1. Copy the content of the file [lightweight-la-code.js](lightweight-la-code.js).
1. Navigate to your course.
1. Having the main page of the course open, open the browser's console.
   - For Google Chrome, open the Chrome Menu in the upper-right-hand corner of the browser window and select More Tools > Developer Tools. You can also use Option + ⌘ + J (on macOS), or Shift + CTRL + J (on Windows/Linux).

   - For Firefox, click on the Firefox Menu in the upper-right-hand corner of the browser and selects More Tools > Browser Console. You can also use the shortcut Shift + ⌘ + J (on macOS) or Shift + CTRL + J (on Windows/Linux).
 
   - For Microsoft Edge, open the Edge Menu in the upper-right-hand corner of the browser window and select More Tools > Developer Tools. You can also press CTRL + Shift + i to open it.
 
   - For other browsers, please check out their documentation.
1. Paste the copied code and execute it (e.g., by pressing the Enter key).

### Moodle Backup Files (mbz) - recommended

#### Step by Step Guide

![](video/moodle-how-to-restore-a-course.webm)

[//]: # (<REPLACE < with open and > with closed paranthesis>For ILIAS some special features have to be considered, Download the `*.mbz`-files <according to your preferred version and language>.)
1. Download the file [lightweight-la-module.mbz](lightweight-la-module.mbz).
1. Navigate to the course reuse settings and pick the restore option.
1. Pick the downloaded `*.mbz`-file in the "Upload File" dialogue.
1. Perform the restore in your Moodle course. Watch out to pick the right option to not delete any existing content of your course during the restore process accidentally.

## License
See the [LICENSE](./LICENSE)-file for license rights and limitations (MIT).