In this Assignment we will cover some basic command of linux

First check your current working directory
pwd

Now create directory with name "linux" in your current directory.
mkdir linux

Then create a another directory with name "Assignment-01" inside your "linux" directory .
mkdir /linux/Assignment-01/

Now create one more directory inside "/tmp" with name "dir1" without changing your present directory.
mkdir /tmp/dir1/

At last create two more directories having below tree structure .It should create a below structure via single command only .
/tmp

- dir1
  - dir2
    - dir3

mkdir -p /tmp/dir1/dir2/dir3/

Find a command that will delete a "dir3" that you have created before.
rmdir /tmp/dir1/dir2/dir3

Now create a empty file with your "firt-name" in /tmp directory.
touch /tmp/Chavi
After creating a empty file , add "This is my first line " into a file without using any editor.

echo "This is my first line " >> file.txt

Now add one more line "this is a additional content " into a same file .Make sure it will not overwrite the previous line of the file.

echo ""this is a additional content " >> file.txt

Then create new file with your "last-name" along with some content like "last-name is my last name".Do not use any editor

echo "suryavanshi is my last name" >> suryavanshi

Now add "this is line at the beginning" into "last-name" file in such a manner that it will add the line at beginning of the file.Do not use any editor.

echo "this is line at the beginning" | cat - suryavanshi > temp && mv temp suryavanshi

Now find a command that will show:

top 5 lines of the file.
head -n 5 suryavanshi

bottom 2 lines of the file.
tail -n 2 suryavanshi

only 6th line of the file.
head -n 6 suryavanshi | tail -n 1

3-8 lines of the file .
head -n 8 suryavanshi | tail -n +3

Find a command that will list below things of /tmp directory
list all content(including hidden files)
ls -a

list only files
ls -p | grep -v /

list only directories
ls -d \*/

Now copy the "last-name" into the /tmp/dir2 with same name.
cp suryavanshi linux/Assignment01/dir1/dir2

Then again copy the "last-name" into the /tmp/dir2, this time with different name i.e "last-name".copy
mv suryavanshi last-name
mv firstname /linux/Assignment01/dir1

Now change the name of the "first-name" file to some other name at same location .
mv aditya first_name

Find a command that will move the "last-name" file to /tmp/dir1
mv /tmp/dir1/dir2/suryavanshi /tmp/dir1/

find a command that will clear the content of /tmp/dir2/"last-name".copy .Make sure it will not even contain empty line.
truncate -s 0 /linux/Assignment01/dir1/aditya

Now delete the same file i.e /tmp/dir2/last-name.copy
rm /linux/Assignment01/dir1/aditya
