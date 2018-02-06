# How to Zip Files Using Terminal in COMP 2402

Use the zip command in the terminal when in the root assignment folder:

    zip -r new_folder.zip folder_1 folder_2 -x "*.DS_Store" "*.class"

This will zip `folder_1` and `folder_2` and their contents [recursively, `-r` command] into a zip file named `new_folder.zip`.

The zip command will compress without the `__MACOSX` folder, which is added when using the system compressing tool. The `*.DS\_Store` and `*.class` arguements are added after the `-x` command to ignore all files that have these file extensions.

## Compiling Java Using Terminal

This command will comiple the java file and output any compilation errors.

    javac PartX.java

## Running Java Programs Using Terminal [Assignment 1]

This command will run the compiled Java code, take the `testX-01.in` file as input and write to the `testX-01.in` file.

java comp2402a1.PartX tests/testX-01.in tests/testX-01.out

### For copying and pasting

    javac Part10.java

    java comp2402a1.Part10 tests/test10-01.in tests/test10-01.out

    zip -r comp2402a1.zip comp2402a1 tests -x "*.DS_Store" "*.class"