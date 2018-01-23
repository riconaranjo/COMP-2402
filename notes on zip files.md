# How to zip files using the terminal for this course

Use the zip command in the terminal when in the root assignment folder:

    zip -r comp2402aX.zip comp2402aX tests -x "*.DS_Store"

The zip command will compress without the __MACOSX folder, which is added when using the system compressing tool. The *.DS\_Store is added to the command to ignore all files that have this file extension.