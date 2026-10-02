# Lightweight LA

This repository offers material to integrate Learning Analytics (LA) into web-based Learning Management Systems (LMS), esp. Moodle, lightweightly. I.e., they can be implemented by lecturers in their courses using the on-board tools of the LMS. Neither plugin installations nor additional technical permissions are required.

## Implementation
The rules, logic and GUI of the tool are contained in a single JavaScript file ([lightweight-la-code.js](lightweight-la-code.js)). There are three ways for lecturers to integrate the tool into their courses.
1. For a first glimpse, the [console-based approach](#console-based---quick) integrates the tool temporarily. It's completely gone when you close the browser window or reload the page.
1. The recommended way is to upload it into the course [via the mbz-module](#moodle-backup-files-mbz---recommended) using Moodle's in-built restore option. This adds an element containing the said JavaScript into your course.
1. Alternatively, you can create an element inside your course and [save the JavaScript code into that element](#save-in-course-element----fallback) by yourself.

### Console-based - Quick
#### Step by Step Guide
1. Copy the content of the file [lightweight-la-code.js](lightweight-la-code.js).
1. Navigate to your course.
1. Having the main page of the course open, open the browser's console.
   - For Google Chrome, open the Chrome Menu in the upper-right-hand corner of the browser window and select More Tools > Developer Tools. You can also use Option + ⌘ + J (on macOS), or Shift + CTRL + J (on Windows/Linux).

   - For Firefox, click on the Firefox Menu in the upper-right-hand corner of the browser and selects More Tools > Browser Console. You can also use the shortcut Shift + ⌘ + J (on macOS) or Shift + CTRL + J (on Windows/Linux).
 
   - For Microsoft Edge, open the Edge Menu in the upper-right-hand corner of the browser window and select More Tools > Developer Tools. You can also press CTRL + Shift + i to open it.
 
   - For other browsers, please check out their documentation.
1. Paste the copied code and execute it (e.g., by pressing the Enter key).

### Moodle Backup Files (mbz) - Recommended

#### Step by Step Guide
[//]: # (<REPLACE < with open and > with closed paranthesis>For ILIAS some special features have to be considered, Download the `*.mbz`-files <according to your preferred version and language>.)
1. Download the file [lightweight-la-module.mbz](lightweight-la-module.mbz).
1. Navigate to your course.
1. To have the code transported by the module work properly, check your course's filter settings. URLs must not be converted. (Usually under More -> Filters -> Convert URLs into links and images -> Off)
1. Import the downloaded module into your course using Moodle's restore option. For how to restore a course, see https://docs.moodle.org/502/en/Course_restore or the following bullet points.
   - Navigate to the course reuse settings and pick the restore option. (Usually under More -> Course reuse -> Restore)
   - Pick the downloaded `*.mbz`-file in the "Upload File" dialogue.
   - Perform the restore in your Moodle course. Watch out to pick the right option to not delete any existing content of your course during the restore process accidentally.

### Save in Course Element  - Fallback

#### Step by Step Guide
1. Copy the content of the file [lightweight-la-code.js](lightweight-la-code.js).
1. Navigate to your course.
1. To have the code transported by the module work properly, check your course's filter settings. URLs must not be converted. (Usually under More -> Filters -> Convert URLs into links and images -> Off)
1. Switch to edit mode.
1. Add a new course activity in which you can store text, e.g., the *Text and Media* element.
1. In the element's text setting, switch to *Source Code* mode. (For TinyMCE editor do, e.g., Tools -> Source Code.)
1. Paste the copied code as source code into the text element.
1. Set the element's availability to *Hidden for Students*.
1. Save the element and return to the course page.

## License
See the [LICENSE](./LICENSE)-file for license rights and limitations (MIT).