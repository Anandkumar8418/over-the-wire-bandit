# over-the-wire-bandit
Self Assessment Task PClub
<!-- Level 0 -->
ssh bandit0@bandit.labs.overthewire.org -p 2220
bandit0(writing password)
ls
cat readme(got the passoword for level1 NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL)

<!-- Level 1 -->
ssh bandit1@bandit.labs.overthewire.org -p 2220
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL(password)
ls
cat < - (to open - file ,password for level2 rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi)

<!-- Level 2 -->
ssh bandit2@bandit.labs.overthewire.org -p 2220
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
ls
cat 'spaces in this filename'(password for level3 aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG)

<!-- Level 3 -->
ssh bandit3@bandit.labs.overthewire.org -p 2220
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
ls
cd inhere
ls -a(to see hidden files)
cat .hidden(password for level4 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe)

<!-- Level 4 -->
ssh bandit4@bandit.labs.overthewire.org -p 2220 
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
ls 
cd inhere
ls
cat < -file00
cat < -file01
cat < -file02
cat < -file03
cat < -file04
cat < -file05
cat < -file06
cat < -file07(only human readable file,password for level5 lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR)
cat < -file08
cat < -file09

<!-- Level 5 -->
ssh bandit5@bandit.labs.overthewire.org -p 2220 
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
ls
cd inhere
ls
find -type f -size 1033c ! -executable -exec grep -Iq . {} \; -exec cat {} \;(finding right file ,password for lvl6 P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU)


<!-- Level 6 -->
ssh bandit6@bandit.labs.overthewire.org -p 2220 
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null ( to find the location of password file)
cat /var/lib/dpkg/info/bandit7.password(to get the password from found file directory , password for file 7 is z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S)

<!-- Level 7 -->
ssh bandit7@bandit.labs.overthewire.org -p 2220 
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
ls(got data.txt)
grep "millionth" data.txt( got password for level8 TESKZC0XvTetK0S9xNwm25STk5iWrBvP)

<!-- Level 8 -->
ssh bandit8@bandit.labs.overthewire.org -p 2220 
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
ls
cat data.txt | sort | uniq -u  ( got password for level9 EN632PlfYiZbn3PhVK3XOGSlNInNE00t)

<!-- Level 9 -->
ssh bandit9@bandit.labs.overthewire.org -p 2220 
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
ls
strings data.txt | grep -oP '=+\s*\K\S+'(to get password from file for lvl 10 G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s)

<!-- Level 10 -->
ssh bandit10@bandit.labs.overthewire.org -p 2220 
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
ls
base64 -d data.txt(got password for lvl11 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM)


<!-- Level 11 -->
ssh bandit11@bandit.labs.overthewire.org -p 2220 
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
ls
tr 'A-Za-z' 'N-ZA-Mn-za-m' < data.txt(got password for level12 JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv)


<!-- Level 12 -->
ssh bandit12@bandit.labs.overthewire.org -p 2220 
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
mkdir /tmp/idk (making temp directory)
cp data.txt /tmp/idk
cd /tmp/idk
xxd -r data.txt > bandit( msg shown bandit: gzip compressed data, was "data2.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix, original size modulo 2^32 581
)
mv bandit bandit.gz
gunzip bandit.gz
file bandit
mv bandit bandit.bz2
bzip2 -d bandit.bz2
file bandit
mv bandit bandit.gz
gunzip bandit.gz
file bandit
mv bandit bandit.tar
tar -xf bandit.tar
file data5.bin
mv data5.bin data5.tar
tar -xf data5.tar
file data6.bin
mv data6.bin data6.bz2 
bzip2 -d data6.bz2
mv data6 data6.tar
tar -xf data6.tar
file data8
mv data8.bin data8.gz
gunzip data8.gz
cat data8 (password for level13 is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw)


<!-- Level 13 -->
ssh bandit13@bandit.labs.overthewire.org -p 2220 
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
ls(sshkey.private)
ssh -i sshkey.private bandit14@localhost -p 2220
cd /etc/bandit_pass/
ls
cat bandit14(i got the password for level 14 fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq)

<!-- Level 14 -->
ssh bandit14@bandit.labs.overthewire.org -p 2220 
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
nc localhost 30000(then i pasted the password for level 14 )
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq( i got the password for level15 jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt)


<!-- Level 15 -->
ssh bandit15@bandit.labs.overthewire.org -p 2220 
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
openssl s_client -connect localhost:30001
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt( i got password of level 16 JQttfApK4SeyHwDlI9SXGR50qclOAil1)
