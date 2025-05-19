<img width="1303" alt="forctype" src="https://github.com/user-attachments/assets/006f0ccf-ca22-42fc-a187-e90a102d76b1" /><img width="1303" alt="forin1" src="https://github.com/user-attachments/assets/f60b48d5-fd73-46fe-98db-d7c95061971e" /><img width="1303" alt="whiletest" src="https://github.com/user-attachments/assets/6cf7a498-7987-4303-8739-f02e6b71b77a" /><img width="1303" alt="catscriptcheck" src="https://github.com/user-attachments/assets/3f8910cb-c80f-4c3e-a982-9ccd93e54224" /><img width="1303" alt="catherecheck" src="https://github.com/user-attachments/assets/d2c34d21-2273-4435-8d58-47278f871c66" /><img width="983" alt="tar2" src="https://github.com/user-attachments/assets/1de40ace-0a5b-4d7e-b07d-5fb998e8d31d" /><img width="983" alt="tar1" src="https://github.com/user-attachments/assets/77256970-eb37-43f4-838f-660abebb859b" /><img width="1172" alt="egrep2" src="https://github.com/user-attachments/assets/b8f62ac1-a464-4de8-a1d0-b78925cb2b74" /># OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
// git add-h
// git commit
// git origin

### Display the content of the files
cat < file1


## OUTPUT
<img width="1581" alt="cat file1" src="https://github.com/user-attachments/assets/99afcafe-27b9-426b-af66-a18d0ece01d7" />

cat < file2
## OUTPUT

<img width="1581" alt="cat file2" src="https://github.com/user-attachments/assets/2c61e255-d9bd-44a3-a274-bbc54929ef60" />


# Comparing Files
cmp file1 file2
## OUTPUT

<img width="1593" alt="comp" src="https://github.com/user-attachments/assets/5947068e-88b7-4e26-ae3b-957d8104b1c6" />

 
comm file1 file2
 ## OUTPUT

<img width="1581" alt="comm" src="https://github.com/user-attachments/assets/51a6fabe-7a39-4008-9dc4-3f1e3e266755" />

 
diff file1 file2
## OUTPUT

<img width="1581" alt="diff" src="https://github.com/user-attachments/assets/83a41610-cc2b-425b-938f-a7653866cac5" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```


cut -c1-3 file11
## OUTPUT

<img width="1581" alt="cut-c1-c3file11" src="https://github.com/user-attachments/assets/1ae328ba-cb86-428b-be06-9b060c05d900" />


cut -d "|" -f 1 file22
## OUTPUT

<img width="1669" alt="cut-d-f1file22" src="https://github.com/user-attachments/assets/51650eb7-8e0a-42a8-9edc-e9e72c160628" />


cut -d "|" -f 2 file22
## OUTPUT

<img width="1669" alt="cut-d-f2file22" src="https://github.com/user-attachments/assets/efc853d4-32f4-4e33-8dad-bd86ab2b0b43" />


cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT


<img width="1669" alt="grepHello" src="https://github.com/user-attachments/assets/3043d351-7e86-481d-92cd-342d28372b92" />

grep hello newfile 
## OUTPUT

<img width="1669" alt="grep_hello" src="https://github.com/user-attachments/assets/8a0bf064-2228-48cc-8f1d-8a5cbb1f7778" />



grep -v hello newfile 
## OUTPUT

<img width="1669" alt="grep-v" src="https://github.com/user-attachments/assets/6bfde94a-950d-4f67-ab81-972a5a87ca13" />


cat newfile | grep -i "hello"
## OUTPUT

<img width="1781" alt="catgrepi" src="https://github.com/user-attachments/assets/eaa7531d-b0ea-4204-8203-3c21cb41a80d" />



cat newfile | grep -i -c "hello"
## OUTPUT

<img width="1827" alt="catgrepic" src="https://github.com/user-attachments/assets/314fa78a-a127-4967-bc79-ed2f5dd40ca4" />



grep -R ubuntu /etc
## OUTPUT

<img width="1039" alt="grep -r ubuntu" src="https://github.com/user-attachments/assets/1ee94382-81ef-4249-8eef-49f6760b9134" />


grep -w -n world newfile   
## OUTPUT

<img width="1108" alt="grep newworld" src="https://github.com/user-attachments/assets/2cf27a63-cc98-44b9-84c3-668e46ce3351" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="1172" alt="egrep1" src="https://github.com/user-attachments/assets/39bc2c0d-99fd-4d9f-ae08-5bbc1091cad9" />


egrep -w '(H|h)ello' newfile 
## OUTPUT

<img width="1172" alt="egrep2" src="https://github.com/user-attachments/assets/1ca4ce6f-afcb-4175-820c-252aea862f1b" />


egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

<img width="1191" alt="egrep3" src="https://github.com/user-attachments/assets/260f3f90-b778-4163-b0be-3e661ac202d2" />



egrep '(^hello)' newfile 
## OUTPUT

<img width="1191" alt="egrep4" src="https://github.com/user-attachments/assets/e4347554-5765-4bfa-a639-a3de6a8c3c18" />


egrep '(world$)' newfile 
## OUTPUT

<img width="1191" alt="egrep5" src="https://github.com/user-attachments/assets/bec26142-2c7e-4465-80ff-89ac73939cb9" />

egrep '(World$)' newfile 
## OUTPUT

<img width="1191" alt="egrep5" src="https://github.com/user-attachments/assets/e535080a-8573-4896-aaef-299443538d21" />

egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="1191" alt="egrep7" src="https://github.com/user-attachments/assets/c128b4d7-7f9a-4857-938d-c5f661bac00e" />


egrep '[1-9]' newfile 
## OUTPUT

<img width="1191" alt="egrep8" src="https://github.com/user-attachments/assets/1d58703d-ecc2-44c7-ba3c-c2bf7d7909e7" />


egrep 'Linux.*world' newfile 
## OUTPUT

<img width="1191" alt="egrep9" src="https://github.com/user-attachments/assets/69e36604-200c-4ba7-aeb1-ff19cb19fe44" />

egrep 'Linux.*World' newfile 
## OUTPUT

<img width="1191" alt="egrep10" src="https://github.com/user-attachments/assets/157a74d1-ca04-4d3a-a8c6-0be30817a9b1" />


egrep l{2} newfile
## OUTPUT

<img width="1191" alt="egrep11" src="https://github.com/user-attachments/assets/ec0156bb-847f-46fe-b840-1567b8809ed4" />


egrep 's{1,2}' newfile
## OUTPUT 

<img width="1191" alt="egrep12" src="https://github.com/user-attachments/assets/7b1b0fab-071b-40b8-b250-7b4ad4c71b51" />

cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```


sed -n -e '3p' file23
## OUTPUT

<img width="1191" alt="sed1" src="https://github.com/user-attachments/assets/3754e811-2dbc-4674-9f9c-459dd12ca78b" />

sed -n -e '$p' file23
## OUTPUT

<img width="1191" alt="sed2" src="https://github.com/user-attachments/assets/10e9990b-805b-4e28-95a2-11d4aea6fb6d" />

sed  -e 's/Ram/Sita/' file23
## OUTPUT

<img width="1191" alt="sed3" src="https://github.com/user-attachments/assets/7a9df339-4101-45aa-b616-cb15a013d3cd" />


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

<img width="1191" alt="sed4" src="https://github.com/user-attachments/assets/75c1a6d1-d592-4bfc-a6e1-79182dfbf780" />

sed  '/tom/s/5000/6000/' file23
## OUTPUT

<img width="1191" alt="sed5" src="https://github.com/user-attachments/assets/4ae4bee8-db86-4b5a-8eef-6e104ae7a167" />


sed -n -e '1,5p' file23
## OUTPUT
<img width="1191" alt="sed6" src="https://github.com/user-attachments/assets/0071cc8f-a4e3-4fbc-a330-7d52542bfc5a" />


sed -n -e '2,/Joe/p' file23
## OUTPUT

<img width="1191" alt="sed7" src="https://github.com/user-attachments/assets/e7a09b4f-075c-4ae9-afa0-86a24e7627e6" />


sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

<img width="1191" alt="sed8" src="https://github.com/user-attachments/assets/a14557ad-6f29-4871-8a85-304c79f123d7" />

seq 10 
## OUTPUT

<img width="1191" alt="seq1" src="https://github.com/user-attachments/assets/752ba498-06a3-4de8-8543-9db294d62f51" />


seq 10 | sed -n '4,6p'
## OUTPUT

<img width="1191" alt="seq2" src="https://github.com/user-attachments/assets/277b89ff-c50a-4527-b249-cda1262fa411" />


seq 10 | sed -n '2,~4p'
## OUTPUT

<img width="1191" alt="seq3" src="https://github.com/user-attachments/assets/77f1c6a0-decf-4746-b1e7-a78f2948df36" />


seq 3 | sed '2a hello'
## OUTPUT

<img width="1191" alt="seq4" src="https://github.com/user-attachments/assets/ad45d334-8e9a-4f37-9f94-9306d9e35392" />


seq 2 | sed '2i hello'
## OUTPUT

<img width="1191" alt="seq5" src="https://github.com/user-attachments/assets/55826fc8-db1a-4a37-b4c9-b2c9b9a79e80" />

seq 10 | sed '2,9c hello'
## OUTPUT

<img width="1191" alt="seq6" src="https://github.com/user-attachments/assets/22993355-82a6-4890-863a-6e18febecb4f" />


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

<img width="1191" alt="seq7" src="https://github.com/user-attachments/assets/cf1e7711-d8ca-49fc-a621-776bc493e7cd" />


sed -n '2,4{s/$/*/;p}' file23

<img width="1191" alt="seq8" src="https://github.com/user-attachments/assets/60d7fe7a-f41f-4201-8a6c-9c6d46514d10" />

#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

<img width="1191" alt="sort" src="https://github.com/user-attachments/assets/c558108c-069a-412e-8cf7-f6faf831c30e" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT

<img width="1191" alt="uniq" src="https://github.com/user-attachments/assets/38c9e3a1-c5cd-4ca3-aeda-f96d61852bc7" />


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

<img width="1220" alt="catfile23" src="https://github.com/user-attachments/assets/6fc4fd97-4d74-48cb-b291-6cbc9240278e" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT

 <img width="1150" alt="caturl1" src="https://github.com/user-attachments/assets/f4f05655-65c0-413f-b76c-8771c729df94" />

cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

<img width="1262" alt="caturl2" src="https://github.com/user-attachments/assets/87562c93-9983-40f0-b0cf-32f7bd7ed910" />

#Backup commands
tar -cvf backup.tar *
## OUTPUT

<img width="983" alt="tar1" src="https://github.com/user-attachments/assets/a0f8ecec-e266-4a07-a486-e5c763bdf81d" />

mkdir backupdir
 
mv backup.tar backupdir
 
## OUTPUT

<img width="983" alt="mv1" src="https://github.com/user-attachments/assets/e2c2ea96-ad75-4b39-bd78-eea8be7447ca" />
ng)

tar -xvf backup.tar
## OUTPUT

<img width="983" alt="tar2" src="https://github.com/user-attachments/assets/7ecb7ede-b412-4088-b233-2566f7abe9eb" />

gzip backup.tar

ls .gz
## OUTPUT

<img width="983" alt="ls1" src="https://github.com/user-attachments/assets/a8a859b9-b847-4d66-b265-b78ced9ede34" />

gunzip backup.tar.gz
## OUTPUT

<img width="1112" alt="ls2" src="https://github.com/user-attachments/assets/91a92486-2638-4591-acfd-e7a1a1210014" />

# Shell<img width="1112" alt="ls2" src="https://github.com/user-attachments/assets/c1383d63-eb36-4374-9d73-33a53b177be4" />
 Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World'; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

<img width="1303" alt="echo1" src="https://github.com/user-attachments/assets/6cf9c113-6a2f-41f4-b253-1eb7fbb3deeb" />

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

<img width="1303" alt="catherecheck" src="https://github.com/user-attachments/assets/d1182951-7f08-40d6-8105-a8775803286b" />

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 <img width="1303" alt="catscriptcheck" src="https://github.com/user-attachments/assets/70861cdb-c31b-4496-b1dd-dc7c0fb0eba4" />

ls file1
## OUTPUT

<img width="1303" alt="ls_1" src="https://github.com/user-attachments/assets/3afd72da-bdae-4214-8e48-d1d8b475dc30" />

echo $?
## OUTPUT 

<img width="1303" alt="echo_1" src="https://github.com/user-attachments/assets/1c99d190-dcf3-4e10-a9bc-622721191a66" />

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 

<img width="1303" alt="echo_3" src="https://github.com/user-attachments/assets/17756935-a34a-4b63-8fc2-d24fc0cdb8b4" />

abcd
 
echo $?
## OUTPUT

<img width="1303" alt="echo_2" src="https://github.com/user-attachments/assets/f00cbba0-8439-48eb-b299-70a46cd285ba" />

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
## OUTPUT

<img width="1303" alt="cat_Strcmp" src="https://github.com/user-attachments/assets/3922d05f-cccd-4e91-8551-130aaa357c7d" />


chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

<img width="1303" alt="strcmp" src="https://github.com/user-attachments/assets/02ac4d59-60fa-4aab-934d-11c3397b89bf" />

# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT

<img width="1303" alt="psswdperm" src="https://github.com/user-attachments/assets/974d5624-3e7d-440b-a9a9-7b718f7a6efe" />


# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

<img width="1303" alt="ifnested" src="https://github.com/user-attachments/assets/79fef4b4-638e-410c-9b50-95df817183c7" />

# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

<img width="1303" alt="iftest" src="https://github.com/user-attachments/assets/c5e356c8-3710-4c26-b853-a33d976d9c79" />

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
<img width="1303" alt="ifnested" src="https://github.com/user-attachments/assets/1ce817a9-dee3-4e74-b109-b343f068a6de" />

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT

<img width="1303" alt="elifcheck" src="https://github.com/user-attachments/assets/8ed3289a-bc26-48ac-a1f1-584937da42af" />

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT

<img width="1303" alt="ifcompound" src="https://github.com/user-attachments/assets/9433b8e1-a69a-4aa2-9d58-7628f9cf904e" />

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
## OUTPUT

<img width="1303" alt="casecheck" src="https://github.com/user-attachments/assets/ba777fe9-4270-4d5b-9875-1a6e84f7c8d5" />

cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
## OUTPUT

 <img width="1303" alt="whiletest" src="https://github.com/user-attachments/assets/66eac430-7466-4a6b-868b-9c3cce9fe1f4" />

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
$ ./untiltest.sh
## OUTPUT

 <img width="1303" alt="untiltest" src="https://github.com/user-attachments/assets/93cd1cc7-98f1-49a3-9760-32fd147a79e6" />

 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
$ ./forin1.sh
## OUTPUT

 <img width="1303" alt="forin1" src="https://github.com/user-attachments/assets/3b7a70e7-76cc-4842-b36b-af2339acb59e" />

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
$ ./forin2.sh
## OUTPUT

 <img width="1303" alt="forin2" src="https://github.com/user-attachments/assets/a664b7c9-24db-49bb-ab94-dc56af9fa22f" />

 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```

$ chmod 755 forin3.sh
$ ./forin3.sh 
## OUTPUT

<img width="1303" alt="forin3" src="https://github.com/user-attachments/assets/19685e41-f596-4f50-bfef-1d525e82a6c7" />

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```

cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

$ chmod 777 forinfile.sh
$./forinfile.sh
## OUTPUT

<img width="1303" alt="forinfile" src="https://github.com/user-attachments/assets/10512cc5-89ce-4f29-b162-63184df44d26" />

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

<img width="1303" alt="forctype" src="https://github.com/user-attachments/assets/76c218c6-abef-468f-8789-82e74a1538ef" />

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype1.sh
$ ./forctype1.sh 
## OUTPUT

<img width="1303" alt="forctype1" src="https://github.com/user-attachments/assets/fc3e1e39-73ae-4051-bc80-62ce6a313db5" />

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 <img width="1303" alt="forneseted1" src="https://github.com/user-attachments/assets/f0df7d38-01d8-4af9-ac66-e57d342a3092" />

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```


$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
## OUTPUT

 <img width="1303" alt="forbreak" src="https://github.com/user-attachments/assets/406789e0-1015-435e-a0f6-3f3ce2c67e32" />

cat forcontinue.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed"
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT

<img width="1303" alt="forcontinue" src="https://github.com/user-attachments/assets/dd7f48b3-d8e4-49df-9e68-dc850aaccd50" />

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

<img width="1303" alt="exread" src="https://github.com/user-attachments/assets/988b9f9d-6ae2-4908-9fac-dc6df08df112" />

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. "
``` 
$ chmod 755 exread1.sh 
$ ./exread1.sh 
## OUTPUT

<img width="1303" alt="exread1" src="https://github.com/user-attachments/assets/f6d2e36e-fbae-4573-a4e2-52bfbc9cba21" />



 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```

## OUTPUT
 ./funcex.sh 

 <img width="1303" alt="funcex" src="https://github.com/user-attachments/assets/7c14a936-640d-4122-b8b7-a0fe9c953043" />

 ./funcex.sh 1 2
![image](https://github.com/user-attachments/assets/65a071e2-fc12-4539-a519-60de9c24e2e6)
 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
![image](https://github.com/user-attachments/assets/4a12e3b5-2874-45e6-9d36-bb73b0224ff9)

 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift1.sh
## OUTPUT
$ ./argshift1.sh 1 2 3
![image](https://github.com/user-attachments/assets/3d1d2619-1a29-49c4-987b-702b62479168)

cat argshift3.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +xch
```
## OUTPUT
 ./argshift3.sh 1 2 3
![image](https://github.com/user-attachments/assets/44d1a2ef-ad86-46cc-813b-04dc27c98def)
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
![alt text](img/awk.png)![image](https://github.com/user-attachments/assets/eee0bac8-2c7f-471a-833c-dfd6bb08a8a4)

 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 

![image](https://github.com/user-attachments/assets/b1e3e280-1c2d-4c17-9049-1799012ce4a3)

# RESULT:
The Commands are executed successfully.
