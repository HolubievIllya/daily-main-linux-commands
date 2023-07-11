## Commands
## ls command
List files and folders in the current directory.
<p>Parameters:</p>
<ul>
  <li><b>–l</b> to list the content as a detailed list</li>
  <li><b>-a</b> display all files (hidden + non-hidden)</li>
</ul>
<p>Example of input: <b>ls -la</b></p>

## cd command
Change directory from the current directory to another one.
<p>Example of input: <b>cd /home</b></p>

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





