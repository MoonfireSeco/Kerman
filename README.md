# Kerman Auto Hack
A neat script to mercilessly hack Codeforces C++ sources during contests

![alt text](https://github.com/MoonfireSeco/Kerman/raw/master/Example.png)

Dependencies:

It should work for both Python 2 and Python 3.
- pip install requests
- pip install psutil
- pip install bs4
- pip install colorama

	
	    Options:

    	-c: The Contest ID to analyze (1033, 1056, ...)
    
		-p: The Problem Letter to analyze (A, B, C, D, ...)
		
		-s: The page on which to start the analysis (1, 2, 3, ...)
		
		-e: The page on which to end the analysis (10, 11, 12, ...)
		
		-u: Login with an username (for automatic hack uploading). You will be prompted for the password
		
		-h/--help: Show this help message
		
		--BatteringRam: Attack a single, user-given, Suspect.cpp file until it breaks
		
		--PoisonRun: Iterate through all the submissions while only testing for Poison files
		

There are 2 important files generated for Kerman: **TestGen.cpp and Config.txt**

- TestGen.cpp: A C++ Source file that should be edited by the user. It's compiled automatically, and it's used to generate random valid tests for the current problem.

- Config.txt: Can store some neat options like the number of tests to run on a submission before declaring it unhackable.
