## Basic linux commands


-  ``ls`` --> The ls command is used to list files or directories in Linux and other Unix-based operating systems.

![image](https://user-images.githubusercontent.com/113226189/217494948-04eb3a8d-750c-4f6d-8351-50dd95d51569.png)


- ``` ls -l ```--> Type the ls -l command to list the contents of the directory in a table format with columns including.

       - content permissions
       - number of links to the content
       - owner of the content
       - group owner of the content
       - size of the content in bytes
       - last modified date / time of the content
       - file or directory name

![image](https://user-images.githubusercontent.com/113226189/217495432-db37eedd-79cd-4e5d-bdab-a2f5dac171e4.png)


- ```ls -a ```--> Type the ls -a command to list files or directories including hidden files or directories. In Linux, anything that begins with a . is considered a hidden file.

![image](https://user-images.githubusercontent.com/113226189/217495809-6a8e26c4-14eb-432f-84ae-aa939240560e.png)


- ```vim``` --> This is a text editor used in Linux. It stands for “Vi Improved”.

![image](https://user-images.githubusercontent.com/113226189/217500237-50940362-9936-4e09-ab37-7be4cb152fd4.png)



```Mostly used modes in VIM:```

   ```Normal mode:```
      This is the default mode in which vim starts. In normal mode, you can use various commands to navigate and edit the text.

   ```Insert mode:``` 
      In insert mode, you can type text into the file. To enter insert mode, press the "i" key. To exit insert mode and return to normal mode, press the "Esc" key.

   ```Command mode:``` 
      In command mode, you can enter commands to perform various actions, such as saving the file or quitting vim. To enter command mode, press the ":" key.


- ```cat: ``` --> This is used to concatenate and display files on the terminal. It can also be used to modify existing ones.

   ```cat -b:``` This adds line numbers to non-blank lines

   ```cat -n:``` This adds line numbers to all lines

   ```cat -s:``` This squeezes blank lines into one line

   ```cat –E:``` This shows $ at the end of the line

![image](https://user-images.githubusercontent.com/113226189/217499633-741e2a3b-af69-4a71-92ac-e0c0074b2298.png)




## Directoy commands
- ```pwd``` --> Print work directory. Gives the present working directory.

![Screenshot_20230208_035249](https://user-images.githubusercontent.com/113226189/217503078-b5f23e3d-6d1c-4d9d-9f49-b2c4a9223c98.png)


- ```cd path_to_directory``` --> Change directory to the provided path.

![Screenshot_20230208_035641](https://user-images.githubusercontent.com/113226189/217503820-8b94226f-5c42-4463-abcd-fb934f0b3aeb.png)


- ```cd ~ ``` or just  ```cd ``` --> Change directory to the home directory.

![Screenshot_20230208_035743](https://user-images.githubusercontent.com/113226189/217504053-6fed0489-c633-4f2e-9e79-c0b486a803e3.png)


- ``` cd - ``` --> Go to the last working directory.

![Screenshot_20230208_035856](https://user-images.githubusercontent.com/113226189/217504322-4196d648-e59f-4e73-945d-cf9564fddba6.png)


- ``` cd ..``` --> Chnage directory to one step back.

![Screenshot_20230208_040053](https://user-images.githubusercontent.com/113226189/217504728-46a8ae48-0799-4e01-99bb-7841f166d8b8.png)


- ``` cd ../..``` --> Use ls ../.. for contents two levels above.

![Screenshot_20230208_040304](https://user-images.githubusercontent.com/113226189/217505165-d6f3b938-e13c-4d85-bbed-44d0c4fb083f.png)


- ``` mkdir  directoryName``` --> Use to make a directory in a specific location

![Screenshot_20230208_041652](https://user-images.githubusercontent.com/113226189/217508381-8235db87-541b-40a3-8a69-efe4d2dd7af8.png)


- ``` mkdir .NewFolder ``` --> Make a hidden directory (also . before a file to make it hidden)

![Screenshot_20230208_041409](https://user-images.githubusercontent.com/113226189/217507900-235bee59-5dcc-41b1-8090-66744ce48853.png)


- ```mkdir A B C D ``` --> Make multiple directories at the same time.


![Screenshot_20230208_041932](https://user-images.githubusercontent.com/113226189/217509003-2ff3461c-caaa-4a55-a03b-4c20a37cec3f.png)


- ```mkdir /home/user/Mydirectory ``` --> make a new folder in a specific location

![Screenshot_20230208_042318](https://user-images.githubusercontent.com/113226189/217509771-81c6f7a8-9678-4fae-8365-e15a035e71e8.png)


- ```mkdir -p  A/B/C/D ``` --> Make a nested directory

![Screenshot_20230208_042742](https://user-images.githubusercontent.com/113226189/217510808-92e1333c-1b63-4772-b745-769ba949094d.png)
