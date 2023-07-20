## Commands
## ls command
List files and folders in the current directory.
<p>Parameters:</p>
<ul>
  <li><b>–l</b> to list the content as a detailed list</li>
  <li><b>-a</b> display all files (hidden + non-hidden)</li>
  <li><b>-r</b> reverses the sorting order for the displayed files and directories</li>
  <li><b>-s</b> sorts the output by file size</li>
  <li><b>-t</b> sorts the output by file modification time</li>
</ul>
<p>Example of input: <b>ls -la</b></p>

## pwd command
Shows current directory
<ul>
  <li><b>-L</b> prints the symbolic path</li>
  <li><b>-P</b> prints the actual path</li>
</ul>
<p>Example of input: <b>pwd</b></p>

## cd command
Change directory from the current directory to another one.
<ul>
  <li><b>~</b> back to main directory</li>
</ul>
<p>Example of input: <b>cd /home</b></p>

## touch command
The touch command is used to create an empty file.
<p>Parameters:</p>
<ul>
  <li><b>–t</b> creates file followed by the time with the following format YYYYMMDDHHMM</li>
</ul>
<p>Example of input: <b>touch -t 202012011200 test1</b></p>

## rm command
You can easily delete single files
<p>Example of input: <b>rm name</b></p>

## cp command
Copy the source to target.
<p>Parameters:</p>
<ul>
  <li><b>–i</b> interactive mode means waiting for the confirmation if there are files on the target, it will be overwritten</li>
  <li><b>-r</b> recursive copy means include subdirectories if they found</li>
</ul>
<p>Example of input: <b>cp –ir sourcedir targetdir</b></p>

## mv command
Move the source to target and remove the source.
<p>Parameters:</p>
<ul>
  <li><b>–i</b> interactive mode means to wait for the confirmation if there are files on the target, it will be overwritten</li>
</ul>
<p>Example of input: <b>mv –i sourceFile targetFile</b></p>

## rm command
Delete file or directory, and you must use –r in case you want to delete a directory.
<p>Parameters:</p>
<ul>
  <li><b>–r</b> recursive delete means delete all subdirectories if found</li>
  <li><b>-i</b> interactive means wait till confirmation</li>
</ul>
<p>Example of input: <b>rm –r anotherDir/</b></p>

## mkdir command
Create a new directory.
<p>Example of input: <b>mkdir NewDir</b></p>

## rmdir command
Delete a directory.
<p>Example of input: <b>rmdir NewDir/</b></p>

## chown command
Change the owner of a file or directory.
<p>Parameters:</p>
<ul>
  <li><b>–R</b> capital R here means to change ownership of all subdirectories if found, and you must use this parameter if you use the command against a directory</li>
</ul>
<p>Example of input: <b>chown –R root:root myDir</b></p>

## chmod command
Change the permission of a file or directory.
<p>Parameters:</p>
<ul>
  <li>The mode which consists of 3 parts, owner, group, and others means what will be the permissions for these modes, and you must specify them</li>
  <lihe mode which consists of 3 parts, owner, group, and others means what will be the permissions for these modes, and you must specify them.

The permission is one of the followings:

Read =4

Write = 2

Execute =1

Every permission represented by a number as shown, and you can combine permissions.</li>
</ul>
<p>Example of input: <b>chmod 755 myfile</b></p>
That means set permission for the file named myfile as follows:
owner: set it to 7, which means 4+2+1 means read+write+execute.
group: set it to 5, which means 4+1 means read+execute.
other: set it to 5, which means 4+1 means read+execute.
Note: execute for a folder, means opening it.

## locate command
To find a file in your system, the locate command will search the system for the pattern you provide..
<p>Example of input: <b>locate myfile</b></p>

## date command
Simply prints today’s date. Just type date on the shell.
<p>Example of input: <b>date</b></p>

## find command
Finds all files with flags you provided.
<p>Example of input: <b>find . -type f -name "*.txt"</b></p>

## echo command
Used to display line of text/string that are passed as an argument.
<p>Example of input: <b>echo "Hello, world!"</b></p>

## df command
Displays the disk space used in the file system.
<ul>
  <li><b>–h</b> displays space in gb and mb</li>
</ul>
<p>Example of input: <b>df"</b></p>

## tar command
Combines several files into an archive and compression if you want.
<ul>
  <li><b>–c</b> create a new archive</li>
  <li><b>-z</b> compress the archive using gzip package</li>
  <li><b>-j</b> compress the archive using the bzip2 package</li>
  <li><b>-v</b> verbose mode means showing the processed files</li>
  <li><b>-f</b> write the output to a file and not to screen</li>
  <li><b>-x</b> unpack files from an archive</li>
</ul>
<p>Example of input: <b>tar –czvf myfiles.tar.gz myfiles</b></p>
This command will pack and compress all files in folder myfiles to a compressed archive named myfiles.tar.gz.
<p>Example of input: <b>tar-xzvf myfiels.tar.gz</b></p>
This command will decompress the archive.

## cat command
Displays file content to screen without limits.
<p>Example of input: <b>cat myfile.txt</b></p>

## tail command
Output the end of a file
<p>Example of input: <b>tail test.txt</b></p>

## less command
Displays file content with a scroll screen so you can navigate between pages using PgUp, PgDn, Home, and End.
<p>Example of input: <b>less myfile</b></p>

## grep command
Searches for a string in the specified files and displays which line contains the matched string.
<ul>
  <li><b>–R</b> recursive search inside subdirectories if found</li>
  <li><b>-i</b> insensitive search and ignore case</li>
  <li><b>-l</b> displays file name, not the text lines</li>
</ul>
<p>Example of input: <b>grep "print" main.py</b></p>

## passwd command
Used to change your user password.
<p>Example of input: <b>passwd</b></p>

## du command
Calculates the disk usage of a file or a directory.
<ul>
  <li><b>–h</b> display human-readable form</li>
  <li><b>-s</b> summarize the output total size</li>
</ul>
<p>Example of input: <b>du –hs /home</b></p>

## reboot command
Reboot the system immediately.
<p>Example of input: <b>reboot</b></p>

## halt command
Shuts down the system, but make sure to close all of your files to avoid data loss.
<p>Example of input: <b>halt</b></p>

## ps command
The ps command lists the currently running process.
<p>Example of input: <b>ps aux</b></p>

## pkill command
Kill a process.
<p>Example of input: <b>pkill processName</b></p>

## nano command
You can edit file, if it doesn't exist command will create new one
<p>Example of input: <b>nano</b></p>

## Get the version of GTK
<p>Example of input: <b>dpkg -s libgtk-3-0|grep '^Version'</b></p>

## sudo command
Runs command as superuser
<p>Example of input: <b>sudo touch</b></p>

## top command
Provides with information about all running processes
<p>Example of input: <b>top</b></p>

## free command
Shows memory usage
<p>Example of input: <b>free -h</b></p>

## tree command
Shows the hierarchy of files and folders in directory
<p>Example of input: <b>tree</b></p>

## ping command
Shows the ping of the website
<ul>
  <li><b>-c amount</b> display ping amount time</li>
</ul>
<p>Example of input: <b>ping www.google.com</b></p>

## host command
Shows the host information about website
<p>Example of input: <b>host website</b></p>

## netstat command
Show all open connections on your ps 
<p>Example of input: <b>netstat</b></p>

## ifconfig command
Shows ip and etc of your pc
<p>Example of input: <b>ifconfig</b></p>

## w command
Shows all users on your machine
<p>Example of input: <b>w</b></p>

## wc command
Finds out the number of newline count, word count, byte and character count in the files specified by the File arguments
<ul>
  <li><b>-l</b> prints the number of lines in a file</li>
  <li><b>-w</b> prints the number of words in a file</li>
  <li><b>-c</b> displays the count of bytes in a file</li>
  <li><b>-m</b> prints the count of characters from a file</li>
  <li><b>-L</b> prints only the length of the longest line in a file</li>
</ul>
<p>Example of input: <b>wc -L</b></p>

## shuf command
Writes a random permutation of the input lines to standard output.
<ul>
  <li><b>-n</b> prints the number of lines in a file</li>
</ul>
<p>Example of input: <b>shuf -n 25 hello.txt</b></p>
