# Symbolic-Links-and-their-Use
This is a tutorial for learning Symbolic Links . 
A symlink is a symbolic Linux/ UNIX link that points to another file or folder on your computer, or a connected file system. This is similar to a Windows shortcut.

Symlinks can take two forms:

Soft links are similar to shortcuts, and can point to another file or directory in any file system.

Hard links are also shortcuts for files and folders, but a hard link cannot be created for a folder or file in a different file system. These can be created in the following way on Linux and Mac operating systems.

ln -s /<path to file/folder to be linked> <path of the link to be created>
ln is the link command. The -s flag specifies that the link should be soft. -s can also be entered as -symbolic. Please note, ln command creates hard links by default.

The next argument is path to the file (or folder) that you want to link. (That is, the file or folder you want to create a shortcut for.)

The last argument is the path to link itself i.e. Where you would like the shortcut to be placed. This could be the Desktop for example (N.B. name= Home folder name):

Linux
ln -s /home/name/Documents/MyFolder /home/name/Desktop/MyFolder
For folders or files with special characters, like spaces, then use quotes around the paths.

ln -s “/home/name/Documents/My Folder” “/home/name/Desktop/MyFolder”
Mac
ln -s /Users/name/Documents/MyFolder /Users/name/Desktop/MyFolder
For folders or files with special characters, like spaces, then use quotes around the paths.

ln -s “/Users/name/Documents/My Folder” “/Users/name/Desktop/My Folder”
If you find that you can’t make a symlink due to permission issues, then prefix the commands above with sudo. The sudo command is an abbreviation of “super user do”, and is quite a dangerous command in the hands of the inexperienced, as it allows programs to be executed as the root user/ administrator.

e.g.

sudo ln -s /home/name/Documents/MyFolder /home/name/Desktop/MyFolder
Taken from © Wellcome Genome Campus Advanced Courses and Scientific Conferences

