# FileManager Documentation



## Console's methods

### promptForString
Takes input and trims/formats it for other methods to take easily.

### sendMessage
Prints _ to the console



## FileManager's methods

### handleUserInput
Prompts for string. Has special commands for asking for help and inputting nothing- otherwise, hands it off to processCommand.

### processCommand
A switch statement for the different functionalities implemented in FileOperator. May prompt for additional user input depending on the command. 

### renameFile
Part of processCommand's switch cases. Renames a given file. Covers edge cases for given file not existing.

### performCopyMove
Part of processCommand's switch cases. Moves a file from one path to another. Covers edge cases for unexpected exceptions.

### sendIntro
Performed in Console's promptForString when the user asks for help. Prints command options.



## FileOperator's methods
Most of processCommand's switch cases.

### list
Lists files in a given folder. Covers edge cases for empty folders and improper paths.

### info
Prints a given file's name, paths, size, creation date, and mutation date. Covers edge cases for improper paths.

### time
Prints current day, month, year, hour, minute, and second.

### createDir
Makes a new folder. Covers edge cases for illegal characters, repeat names, and unexpected exceptions.

### checkForIllegalChars
Checks input for disallowed characters.

### rename
Changes a given folder's name. Covers edge cases for repeat names and unexpected exceptions.

### copyCut
Depending on user input, will either move or copy a given file to a new location. Covers edge cases for unexpected exceptions.

### delete
Deletes both files and folders of the user's choice. Covers edge cases for given file not existing.

### deleteDir
Deletes the entire directory.

### copyCutDir
Cuts out one directory and copies it to a new locations.

### mkDir
Creates a new directory.






