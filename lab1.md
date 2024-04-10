# Lab Report 1 - Remote Access and FileSystem

## Using ```cd```
```
luishernandez@Luiss-MacBook-Pro-2 ~ % cd
luishernandez@Luiss-MacBook-Pro-2 ~ % 
```

The Absolute path before the command was ran was ```/Users/luishernandez```
The command had no output due to us having no argument in the command.
Since `cd` means change directory, not providing an argument means we do not change the directory.
This leaves us at our home directory.
There was no error created.


```
luishernandez@Luiss-MacBook-Pro-2 ~ % cd lecture1
luishernandez@Luiss-MacBook-Pro-2 lecture1 % 
```
My absolute path before running the command was ```/Users/luishernandez```
THe command changed the directory to `lecture1`.
This was due to us providing an argument, `lecture1`
This output did not create an error due to `lecture1`  being a directory that could be reached.


```
luishernandez@Luiss-MacBook-Pro-2 lecture1 % cd Hello.java
cd: not a directory: Hello.java
luishernandez@Luiss-MacBook-Pro-2 lecture1 % 
```
My absolute path before running the command was ```/Users/luishernandez/lecture1```
The command did not have any output due to the command creating an error.
This command created an error as `cd` means to change directory, but since I providied a file.
Since `cd` is looking for a directory and not a file, this causes an error. 


## Using ```ls```
```
luishernandez@Luiss-MacBook-Pro-2 ~ % ls
Applications            Downloads               Pictures                fun_With_CoPilot        lecture1
CSE_8A_LAB              Library                 Project_2               helloworld.java         project_1
Desktop                 Movies                  Public                  how.java                project_3
Documents               Music                   SearchEngine.java       javacse8b               wavelet
luishernandez@Luiss-MacBook-Pro-2 ~ %
```

My absolute path before running the command was ```/Users/luishernandez```
The command `ls` without any arguments outputed all files in my home directory.
Since the terminal when created starts in the home directory, using `ls` with no arguments makes it so that it will have to list all the directories and files in the current working directory.
The command did not create an error because there was a directory that it was connected to.


```
luishernandez@Luiss-MacBook-Pro-2 ~ % ls lecture1
Hello.class     Hello.java      README          messages
luishernandez@Luiss-MacBook-Pro-2 ~ % 
```
My absolute path before running the command was ```/Users/luishernandez```
The command with the command `lecture1` displayed all of the files in the `lecture1` directory.
This did not create an error due to lecture1 being a valid directory it could access.


```
luishernandez@Luiss-MacBook-Pro-2 ~ % ls helloworld.java
helloworld.java
luishernandez@Luiss-MacBook-Pro-2 ~ % 
```
My absolute path before running the command was ```/Users/luishernandez```
The output of this command was just `helloworld.java`
This command did not have an error due as it followed the correct directory path
from the home directory to the `helloworld.java` file.


## Using ```cat```

```
luishernandez@Luiss-MacBook-Pro-2 ~ % cat

```
My absolute path before running the command `cat` was `/Users/luishernandez`
There was no output of this command.
The command did not show any error.


```
luishernandez@Luiss-MacBook-Pro-2 ~ % cat lecture1
cat: lecture1: Is a directory
```
My absolute path before ruuning the command was `/Users/luishernandez`
The output described that `lecture1` was that a directory
The output was an error that since `lecture` is a directory and not a file.
Since it is not a file it cannot display the contents, causing an error.



```
luishernandez@Luiss-MacBook-Pro-2 lecture1 % cat ~/lecture1/Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
}%                                                                                                                                   
luishernandez@Luiss-MacBook-Pro-2 lecture1 % 

```
My absolutute path before running this command was `/Users/luishernandez`
The output displayed all of the contents that were in the `Hello.java` java
Since we only provided one file it only displayed the contents of the file we provided.
This did not cause any errors.
