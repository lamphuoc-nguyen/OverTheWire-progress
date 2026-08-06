# OverTheWire-progress
In this repository contain the txt file answer of overthewire.org for each level

OTHERWIRE.org 
level 0: 
	-ssh -p 2220 bandit0@bandit.labs.overthewire.org
	 password: bandit0
level 1:
	-ls
	 cat readme
		password: you can see in the response
		exit
		-ssh -p 2220 bandit1@bandit.labs.overthewire.org
		
level 2: "-" is a read file so to read use:
	- cat ./- (while - is -filename)
	password:  you can see in the response
	exit
	-ssh -p 2220 bandit2@bandit.labs.overthewire.org
level 3: "--" 
	- cat -- "--space in this filename--"
	password:  you can see in the response
	exit 
	-ssh -p 2220 bandit3@bandit.labs.overthewire.org
level 4: hiding file: 
	- ls -a (list -all)
	-cat ...Hiding-From-You
	password:  you can see in the response
 	exit 
	-ssh -p 2220 bandit4@bandit.labs.overthewire.org
level 5: only human read using -f
	cd inhere
	ls -a
	cat -- -file07
	password :  you can see in the response
	exit 
	-ssh -p 2220 bandit5@bandit.labs.overthewire.org
level 6: human-readable , 1033byte, not executable : use "find ." recursive 	through folder, sort by file "-type f", "-size 1033c" 1033 byte, not 	executable to use "! executable" 
	-find . -type f -size 1033c ! -executable
	-cat ./maybehere07/.file2
	password:  you can see in the response
	exit 
	-ssh -p 2220 bandit6@bandit.labs.overthewire.org

