# 
#syncbreeze_buffer overflow
 This repo contains the python based fuzzing scripts and exploits.
 That are used to leverage an remote buffer overflow vulnerability in the syncbreeze 10.0.28 application.
 Coded by Nitin.

# Process
STEP-1: Download Syncbreeze enterprise from exploit db https://www.exploit-db.com/exploits/42928 from here and install it in your local windows 32 bit machine
        Run the application and setup a local web server on port 80
        Then login to your kali machine and then connect to local server setup on port 80 using kalis firefox
        Try to capture POST http packets and examine it with the given scripts.
STEP-2: Install immunity debugger on windows machine and then run it as administrator and then open the syncbreeze enterprise application
        and press F9 for execution , observe the EIP register values.
STEP-3: Update the ip adress details with your machine ip and the run the 1-poc.py script using kali terminal or vscode.
        Check wheter the EIP register changed or not we wil observe that the syncbreeze application is stopped or crashed and you can see that the stack 
        gets overflowed with A's.
 
