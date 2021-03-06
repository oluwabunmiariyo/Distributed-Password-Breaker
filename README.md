# Distributed-Password-Breaker

Project: Computer Network and Distributed Systems
Prof: Dr. Christopher Ivancic
Course: CSCI 5363 - 001

# Problem to solve
Here are 3 MD5 hash digests all made from passwords. I am to brute-force the passwords used to generate the MD5 digests.
•	4506ca152a692ca44a41998450f583f4
•	0339bb475c721e705f7fdab0ec6e74f
• 866e6c84d48d529faef1f3a062eb2082

The character space for the passwords are as follows
•	Password can be 4 and 5 characters long
•	Can be any combination from the sets A-Z,a-z,0-9,!@#$%


# What my code does
One way to speed up this process of brute forcing is to have multiple machines brute force a subset of passwords so I produced a program that will give this task to at least 2 VMs (Ubuntu) to do the work and is coordinated by the host (Windows). Each VM brute-forced over a different range of characters until one hash is found. Upon finding the password, the VM will notify the host and have the host terminate the process.


# Direction on how to run program
You can rename Server Code, Client1 Code and Client2 Code as server.py, client1.py and client2.py respectively
open directory where your code is located
execute in cmd : py server.py
execute in terminal : python3 client1.py
execute in terminal : python3 client2.py


# References
The resources from the following URLs helped me complete this project:
•	Youtube: https://www.youtube.com/watch?v=H_Yx73upCuY&t=3s
•	Stack Overflow: https://stackoverflow.com/questions/1557571/how-do-i-get-time-of-a-python-programs-execution
•	Real Python: https://realpython.com/python-sockets/
•	GeeksforGeeks: https://www.geeksforgeeks.org/permutation-and-combination-in-python/


