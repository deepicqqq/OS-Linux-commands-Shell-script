## OS-Linux-commands-Shell-scripting
## Operating systems Lab exercise

## Linux commands-Shell scripting
## Linux commands-Shell scripting

## AIM:
To practice Linux Commands and Shell Scripting

## DESIGN STEPS:

## Step 1:
Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

## Step 2:
Execute the following commands

## Step 3:
Testing the commands for the desired output.

## COMMANDS:
## Create the following files file1, file2 as follows:
cat > file1

chanchal singhvi c.k. shukla s.n. dasgupta sumit chakrobarty ^d

cat > file2

anil aggarwal barun sengupta c.k. shukla lalit chowdury s.n. dasgupta ^d

## Display the content of the files
cat < file1

OUTPUT
chanchal singhvi c.k. shukla s.n. dasgupta sumit chakrobarty ^d

cat < file2

OUTPUT
cat > file2

anil aggarwal barun sengupta c.k. shukla lalit chowdury s.n. dasgupta ^d

## Comparing Files
cmp file1 file2

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/d55c94ad-354c-48f0-96fe-d72266ba643c)

## comm file1 file2

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/772c5412-d2b2-4243-9ef5-7b6cdb42ad7b)


diff file1 file2

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/791eda55-7e83-4d0e-8f4b-32423bbd800e)


#Filters

## Create the following files file11, file22 as follows:
cat > file11

Hello world This is my world ^d

cat > file22

1001 | Ram | 10000 | HR 1002 | tom | 5000 | Admin 1003 | Joe | 7000 | Developer ^d

cut -c1-3 file11

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/b9596472-2f4c-4a85-875f-47896fac9c5e)

cut -d "|" -f 1 file22

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/027c8930-32aa-435e-bcc6-023ee075aa5e)

cut -d "|" -f 2 file22

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/01e4acd3-ae00-44a9-b309-66e2fed72dc0)

cat < newfile

Hello world hello world ^d ` cat > newfile Hello world hello world

grep Hello newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/f3444f04-d5af-4945-9769-8a1c09f18dc6)

 ## grep hello newfile

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/6534c553-a131-4431-93ae-72ba9ad044f5)


grep -v hello newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/75d95a2d-15ea-41bf-8838-af613427a451)

cat newfile | grep -i "hello"

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/b2ab7835-b94f-41ea-aa08-fde797fac725)


cat newfile | grep -i -c "hello"

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/2bd738c3-6a39-498d-aa11-25397cee923b)


grep -R ubuntu /etc

## OUTPUT

grep -w -n world newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/625a66ca-45c6-418c-a06a-67572fc5ba19)


cat < newfile

Hello world hello world Linux is world number 1 Unix is predecessor Linux is best in this World ^d

cat > newfile

Hello world hello world Linux is world number 1 Unix is predecessor Linux is best in this World ^d

egrep -w 'Hello|hello' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/d0597067-9f53-4ad3-8ddc-831f0eafcca6)


egrep -w '(H|h)ello' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/12ac5cd2-e919-4389-92a6-30fd13a7c83a)


egrep -w '(H|h)ell[a-z]' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/4439e9d2-00b2-41a8-9ff2-47eb74428b60)


egrep '(^hello)' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/77263fe6-67b9-4100-a5f8-3eeb70cc93aa)


egrep '(world$)' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/325dd584-1810-4f5b-bfce-0998fd72ce61)


egrep '(World$)' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/cb514de0-526c-4aa6-b552-d0655fea527b)


egrep '((W|w)orld$)' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/add5a5a5-b475-4ddc-85ea-9205f9058bd2)


egrep '[1-9]' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/083ed63b-8740-4353-b3ae-aeacf1873e76)


egrep 'Linux.*world' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/58f0b15a-2307-4aa0-9032-fd189bc43920)


egrep 'Linux.*World' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/94904ccf-560f-45b4-afbf-651dbe011ae5)


egrep l{2} newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/efe3187f-8655-40b4-bb60-e2e7e6cbf7ba)


egrep 's{1,2}' newfile

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/87327d01-af6c-4ec4-a44b-ad3ebf8f544e)


cat > file23

1001 | Ram | 10000 | HR 1001 | Ram | 10000 | HR 1002 | tom | 5000 | Admin 1003 | Joe | 7000 | Developer 1005 | Sam | 5000 | HR 1004 | Sit | 7000 | Dev 1003 | Joe | 7000 | Developer 1001 | Ram | 10000 | HR ^d

sed -n -e '3p' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/6ee1b054-38f9-408a-8c18-74da280efd07)


sed -n -e '$p' file23

OUTPUT
sed -e 's/Ram/Sita/' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/2b84c7d5-85ae-430d-bb7d-fb1f45a754ce)


sed -e '2s/Ram/Sita/' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/65db9d11-a7ca-4a9a-83aa-fb7d6f28f19f)


sed '/tom/s/5000/6000/' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/b40a7a3d-d654-49d4-b08f-3ed14e14e387)


sed -n -e '1,5p' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/9eda430b-98f1-4a5e-b94e-7a6435973700)

sed -n -e '2,/Joe/p' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/224a9d26-ae6d-420a-92a4-442796ca2066)


sed -n -e '/tom/,/Joe/p' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/47fe518c-c58d-47e2-adae-176f7f7a6dc6)


seq 10

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/fab6f2ab-d5a5-479f-8aeb-9e3fb72c4204)


seq 10 | sed -n '4,6p'

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/55199015-ea96-4219-bf6f-8fffc5928a26)


seq 10 | sed -n '2,~4p'

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/39d41f24-375b-49cf-a32e-6ecf76484425)


seq 3 | sed '2a hello'

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/1e2d7448-d9e7-4203-ae81-73fbc66c18a5)


seq 2 | sed '2i hello' ##OUTPUT 304768296-37f79adc-6b21-4499-bbfa-d74aeae1461a

seq 10 | sed '2,9c hello'

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/81b05c77-a8e1-4a2f-9f89-a81c79a80da4)


sed -n '2,4{s/^/$/;p}' file23

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/729e8e4d-f395-42e6-b148-11681020076a)


sed -n '2,4{s/$/*/;p}' file23 ##OUTPUT

304769027-3459be51-4d3f-4d3b-a8ad-e63a1fcadd62

# Sorting File content cat > file21

1001 | Ram | 10000 | HR 1002 | tom | 5000 | Admin 1003 | Joe | 7000 | Developer 1005 | Sam | 5000 | HR 1004 | Sit | 7000 | Dev

sort file21

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/cc476845-d60e-4ad3-a4fc-6adaa13a6c5c)


cat > file22

1001 | Ram | 10000 | HR 1001 | Ram | 10000 | HR 1002 | tom | 5000 | Admin 1003 | Joe | 7000 | Developer 1005 | Sam | 5000 | HR 1004 | Sit | 7000 | Dev

uniq file22

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/34b1c87e-31cf-4425-9160-43dd551fa3a4)


# Using tr command

cat file23 | tr [:lower:] [:upper:]

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/01dda3c2-7fbe-47dd-9f17-79f5726103b1)


cat < urllist.txt

www. yahoo. com www. google. com www. mrcet.... com ^d

cat > urllist.txt

www. yahoo. com www. google. com www. mrcet.... com

cat urllist.txt | tr -d ' '

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/76ef4efb-ff97-4c6d-bb76-46ec794e9dc4)


cat urllist.txt | tr -d ' ' | tr -s '.'

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/c63e4799-e306-4941-bdf1-934ad7e19e30)


#Backup commands tar -cvf backup.tar *

## OUTPUT

![image](https://github.com/22008686/OS-Linux-commands-Shell-script/assets/118916413/e6690b38-43fe-4343-96dc-1c79ca5aa8a0)


mkdir backupdir

mv backup.tar backupdir

tar -tvf backup.tar

## OUTPUT

tar -xvf backup.tar

## OUTPUT

gzip backup.tar ls .gz

## OUTPUT

gunzip backup.tar.gz

## OUTPUT

## Shell Script

echo '#!/bin/sh' > my-script.sh echo 'echo Hello World‘; exit 0 >> my-script.sh

chmod 755 my-script.sh ./my-script.sh

## OUTPUT

cat << stop > herecheck.txt

hello in this world i cant stop for this non stop movement stop

cat herecheck.txt

## OUTPUT

cat < scriptest.sh bash #!/bin/sh echo “File name is $0 ” echo "File name is " basename $0 echo “First arg. is ” $1 echo “Second arg. is ” $2 echo “Third arg. is ” $3 echo “Fourth arg. is ” 
@ is ' 
# is '
You can't use 'macro parameter character #' in math mode
$1#
echo 'The $$ is ' $$ ps ^d

cat scriptest.sh bash #!/bin/sh echo “File name is $0 ” echo "File name is " basename $0 echo “First arg. is ” $1 echo “Second arg. is ” $2 echo “Third arg. is ” $3 echo “Fourth arg. is ” 
@ is ' 
# is '
You can't use 'macro parameter character #' in math mode
$#
echo 'The $$ is ' $$ ps

chmod 777 scriptest.sh

./scriptest.sh 1 2 3

## OUTPUT

ls file1

## OUTPUT

echo $?

## OUTPUT

./one bash: ./one: Permission denied echo $?

## OUTPUT

abcd echo $?

## OUTPUT
## mis-using string comparisons
cat < strcomp.sh bash #!/bin/bash val1=baseball val2=hockey if [ $val1 > $val2 ] then echo "$val1 is greater than $val2" else echo "$val1 is less than $val2" fi ^d

cat strcomp.sh bash #!/bin/bash val1=baseball val2=hockey if [ $val1 > $val2 ] then echo "$val1 is greater than $val2" else echo "$val1 is less than $val2" fi

## OUTPUT 

chmod 755 strcomp.sh

./strcomp.sh

## OUTPUT
## check file ownership
cat < psswdperm.sh bash #!/bin/bash if [ -O /etc/passwd ] then echo “You are the owner of the /etc/passwd file” else echo “Sorry, you are not the owner of the /etc/passwd file” fi ^d

cat psswdperm.sh bash /#!/bin/bash if [ -O /etc/passwd ] then echo “You are the owner of the /etc/passwd file” else echo “Sorry, you are not the owner of the /etc/passwd file” fi

./psswdperm.sh

## OUTPUT
## check if with file location
cat>ifnested.sh bash #!/bin/bash if [ -e $HOME ] then echo “$HOME The object exists, is it a file?” if [ -f $HOME ] then echo “Yes,$HOME it is a file!” else echo “No,$HOME it is not a file!” if [ -f $HOME/.bash_history ] then echo “But $HOME/.bash_history is a file!” fi fi else echo “Sorry, the object does not exist” fi ^d

cat ifnested.sh

#!/bin/bash if [ -e $HOME ] then echo “$HOME The object exists, is it a file?” if [ -f $HOME ] then echo “Yes,$HOME it is a file!” else echo “No,$HOME it is not a file!” if [ -f $HOME/.bash_history ] then echo “But $HOME/.bash_history is a file!” fi fi else echo “Sorry, the object does not exist” fi

./ifnested.sh

## OUTPUT
## using numeric test comparisons
cat > iftest.sh bash #!/bin/bash val1=10 val2=11 if [ $val1 -gt 5 ] then echo “The test value $val1 is greater than 5” fi if [ $val1 -eq $val2 ] then echo “The values are equal” else echo “The values are different” fi ^d

cat iftest.sh bash #!/bin/bash val1=10 val2=11 if [ $val1 -gt 5 ] then echo “The test value $val1 is greater than 5” fi if [ $val1 -eq $val2 ] then echo “The values are equal” else echo “The values are different” fi

$ chmod 755 iftest.sh

$ ./iftest.sh ##OUTPUT

## check if a file
cat > ifnested.sh bash #!/bin/bash if [ -e $HOME ] then echo “$HOME The object exists, is it a file?” if [ -f $HOME ] then echo “Yes,$HOME it is a file!” else echo “No,$HOME it is not a file!” if [ -f $HOME/.bash_history ] then echo “But $HOME/.bash_history is a file!” fi fi else echo “Sorry, the object does not exist” fi ^d

cat ifnested.sh bash #!/bin/bash if [ -e $HOME ] then echo “$HOME The object exists, is it a file?” if [ -f $HOME ] then echo “Yes,$HOME it is a file!” else echo “No,$HOME it is not a file!” if [ -f $HOME/.bash_history ] then echo “But $HOME/.bash_history is a file!” fi fi else echo “Sorry, the object does not exist” fi

$ chmod 755 ifnested.sh $ ./ifnested.sh ##OUTPUT

## looking for a possible value using elif
cat elifcheck.sh bash #!/bin/bash if [ $USER = Ram ] then echo "Welcome $USER" echo "Please enjoy your visit" elif [ $USER = Rahim ] then echo "Welcome $USER" echo "Please enjoy your visit" elif [ $USER = Robert ] then echo "Special testing account" elif [ $USER = gganesh ] then echo "$USER, Do not forget to logout when you're done" else echo "Sorry, you are not allowed here" fi

$ chmod 755 elifcheck.sh $ ./elifcheck.sh

## OUTPUT
## testing compound comparisons
cat> ifcompound.sh bash #!/bin/bash if [ -d $HOME ] && [ -w $HOME ] then echo "The file exists and you can write to it" else echo "I cannot write to the file" fi

$ chmod 755 ifcompound.sh $ ./ifcompound.sh

## OUTPUT
## using the case command
cat >casecheck.sh bash case $USER in Ram | Robert) echo "Welcome, $USER" echo "Please enjoy your visit";; Rahim) echo "Special testing account";; gganesh) echo "$USER, Do not forget to log off when you're done";; *) echo "Sorry, you are not allowed here";; esac

$ chmod 755 casecheck.sh $ ./casecheck.sh cat > whiletest bash #!/bin/bash #while command test var1=10 while [ $var1 -gt 0 ] do echo 
[ $var1 - 1 ] done

$ chmod 755 whiletest.sh

$ ./whiletest.sh

cat untiltest.sh bash #using the until command var1=100 until [ $var1 -eq 0 ] do echo 
[ $var1 - 25 ] done

$ chmod 755 untiltest.sh

cat forin1.sh bash #!/bin/bash #basic for command for test in Alabama Alaska Arizona Arkansas California Colorado do echo The next state is $test done

$ chmod 755 forin1.sh

cat forin2.sh bash #!/bin/bash # another example of how not to use the for command for test in I don't know if this'll work do echo “word:$test” done

$ chmod 755 forin2.sh

cat forin2.sh bash #!/bin/bash # another example of how not to use the for command for test in I don't know if this'll work do echo “word:$test” done

$ chmod 755 forin2.sh

$ ./forin2.sh

cat forin3.sh bash #!/bin/bash # another example of how not to use the for command for test in I don't know if "this'll" work do echo "word:$test" done

$ ./forin3.sh

cat forin1.sh bash #!/bin/bash

## basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado do echo The next state is $test done

$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh bash #!/bin/bash

## reading values from a file
file="cities" for state in cat $file do echo "Visit beautiful $file“ done

$ chmod 777 forinfile.sh $ cat cities Hyderabad Alampur Basara Warangal Adilabad Bhadrachalam Khammam

## OUTPUT
cat forctype.sh bash #!/bin/bash

## testing the C-style 
## for loop
for (( i=1; i <= 5; i++ )) do echo "The value of i is 
 chmod 755 forctype.sh $ ./forctype.sh

## OUTPUT
cat forctype1.sh bash #!/bin/bash

## multiple variables
for (( a=1, b=5; a <= 5; a++, b-- )) do echo "$a - $b" done

$ chmod 755 forctype.sh $ ./forctype1.sh

## OUTPUT
cat fornested1.sh bash #!/bin/bash

## nesting for loops
for (( a = 1; a <= 3; a++ )) do echo "Starting loop $a:" for (( b = 1; b <= 3; b++ )) do echo " Inside loop: $b" done done

$ chmod 755 fornested1.sh

$ ./fornested1.sh

## OUTPUT
cat forbreak.sh bash #!/bin/bash

## breaking out of a for loop
for var1 in 1 2 3 4 5 do if [ $var1 -eq 3 ] then break fi echo "Iteration number: $var1" done echo "The for loop is completed“

## OUTPUT
$ chmod 755 forbreak.sh

$ ./forbreak.sh

cat forbreak.sh bash #!/bin/bash

## breaking out of a for loop
for var1 in 1 2 3 4 5 do if [ $var1 -eq 3 ] then continue fi echo "Iteration number: $var1" done echo "The for loop is completed“

$ chmod 755 forcontinue.sh

$ ./forcontinue.sh

## OUTPUT
cat exread.sh bash #!/bin/bash

## testing the read command
echo -n "Enter your name: " read name echo "Hello $name, welcome to my program. "

$ chmod 755 exread.sh

$ ./exread.sh

## OUTPUT
cat exread1.sh bash #!/bin/bash

## testing the read command
read -p "Enter your name: " name echo "Hello $name, welcome to my program. “

$ chmod 755 exread1.sh

## OUTPUT
$ ./exread1.sh

cat funcex.sh bash #!/bin/bash

trying to access script parameters inside a function
function func { echo $[ $1 *
Extra close brace or missing open brace
$2 ]
}
if [ $# -eq 2 ] then value=func $1 $2 echo "The result is $value" else echo "Usage: badtest1 a b" fi

## OUTPUT
./funcex.sh ./funcex.sh 1 2 cat argshift.sh bash #!/bin/bash while (( "$#" )); do echo $1 shift done

$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3

cat argshift1.sh bash #/bin/bash

store arguments in a special array
args=("$@")

## get number of elements
ELEMENTS=${#args[@]}

## echo each element in array
for loop
for (( i=0;i<$ELEMENTS;i++)); do echo ${args[${i}]} done

$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3

cat argshift.sh bash #!/bin/bash set -x while (( "$#" )); do echo $1 shift done set +x

## OUTPUT
./argshift.sh 1 2 3 cat > nc.awk bash BEGIN{} { print len=length($0),"\t",$0 wordcount+=NF chrcnt+=len } END { print "total characters",chrcnt print "Number of Lines are",NR print "No of Words count:",wordcount }

cat>data.dat bash bcdfghj abcdfghj bcdfghj ebcdfghj bcdfghj ibcdfghj bcdfghj obcdfghj bcdfghj ubcdfghj

awk -f nc.awk data.dat

## OUTPUT
cat > palindrome.sh bash #num=545 echo "Enter the number" read num s=0 rev="" temp=$num while [
You can't use 'macro parameter character #' in math mode
$num -gt 0 ]
do
# Get Remainder
s=$((
You can't use 'macro parameter character #' in math mode
$num % 10 ))
# Get next digit
num=$((
You can't use 'macro parameter character #' in math mode
$num / 10 ))
# Store previous number and
# current digit in reverse
rev=$( echo ${rev}${s} ) done if [ $temp -eq $rev ]; then echo "Number is palindrome" else echo "Number is NOT palindrome" fi


## RESULT:

The Commands are executed successfully.
