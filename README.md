# Kali Linux Command


1. **Username Check** > <code>whoami</code>
2. **Help for** > <code>nmap -h/help</code>
3. **any search for** > <code>locate **(name)**</code>
4. **any folder delete for** > <code>rem -r **(name)**</code>
5. **show hello** > <code>echo 'hello'</code>
6. **create file hello adding in file** > <code>echo 'hello' > new.txt</code>
7. **new line adding in file** > <code>echo 'Bangladesh' >> new.txt</code>
8. **file clear and new text adding** > <code>echo 'Bangladesh' > new.txt</code>
9. **file all text show** > <code>cat new.txt</code>
10. **text show one page go to next page _(Space button)_** > <code>less new.txt</code>
11. **show first 10 line text** > <code>head new.txt</code>
12. **show last 10 line text** > <code>tail new.txt</code>
13. **if you found any word in file** > <code>grep -w 'admin' new.txt</code>
14. **if your found line number and word** > <code>grep -n 'admin' new.txt</code>
15. **open file and modify** > <code>nano new.txt</code>
16. **user type check** > <code>sudo -i</code>
17. **normal user to move root user** > <code>sudo su</code>
18. **if your back to normal user** > <code>su -username</code>
19. **file permission check** > <code>ls -l</code>
20. **file permission remove** > <code>chmod a-w file name</code>
21. **file permission adding** > <code>chmod u+w file name</code>
22. **execute** > <code>chmod u+x file name</code>
23. **install python file** > <code>python filename.py</code>
24. **any <code>deb</code> file install for** > <code>sudo dpkg -i filename</code>
25. **sheel file install for go to folder** > <code>./filename.sh</code>
26. **all file update** > <code>apt upgrade</code>
27. **all file download** > <code>sudo apt upgrade</code>
28. **terminal busy 10 second** > <code>sleep 10</code>
29. **how many process list check complete** > <code>jobs</code>
30. **process running list check** > <code>ps</code>
31. **command last if you adding <code>&</code> running** > <code>**Explen:-** sleep 10&</code> _Show running id number_
32. **If you running file stop** > <code>kill</code>
33. **running file check** > <code>fg</code>
34. **packet send unlimited request** > <code>ping scanme.nmap.org</code>
35. **running 4 packet request** > <code>pign scanme.nmap.org -c 4</code>
36. **show ip address** > <code>ifconfig</code>
37. **kali linux internet disconnect** > <code>sudo ifconfig eth0 down</code>
38. **kali linux internet connect** > <code>sudo ifconfig eth0 up</code>
39. **website Ip address show** > <code>>host website link</code>
40. **username show** > <code>hostname</code>
41. **Change user name** > <code>sudo hostname -b newUserName</code>

42. **<code>(.)</code>mining will search for files from the folder I'm working in** > <code>find. -name filename</code>

43. **The selected folder will show files from that folder** > <code>find /home/kali -name filename</code>

44. **<code>(/)</code> Mining will search for files from the Road folder** > <code>find / -name filename</code>

45. **<code>(*)</code> Mining will show all the files with the file name I gave it** > <code>find /home/kali -name filename*</code>

46. **<code>(*.txt) </code>Mining will show all txt file I gave it** > <code>find /home/kali -name *.txt</code>

47. **<code>(.)</code> <code>(/home/kali)</code> Mining will search from within the two folders** > <code>find . /home/kali -name *.txt -type f</code>

48. **(-perm) Mining will search Permition file ( / u = r ) u - user - file and r - read - file** > <code>find. /home/kali -type f -perm /u=r</code>

49. **<code>(/u=x)</code> Mining execute file** > <code>find . /home/kali -type f -perm /u=x</code>

50. **<code>(0 size)</code> Mining will search 0 size file** > <code>find /home/kali -type -type f -size 0</code>

51. **search and delete** > <code>find /home/kali -type f -size 0 -exec rm/0 size</code>

52. **it will search file and delete all file** > <code>find /home/kali -type f -name *.txt -exec rm/txt</code>

53. **It will search file names related to two types of file show** > <code>find. -type f \(-name '*.log' -o -name '*.php' -o -name filename\)</code>

54. **it will search all file show two type file** > <code>find . -type f \(-name '*.log' -o -name '*.php'\)</code>

55. **** > <code>find . -type f \(-name '*.log' -o -name '*.php' -o -name filename \) -exec rm {}\;</code>

## Nmap
### Nmap Scan  very slowly but can show information very accurately

1. **show details** > <code>nmap -p 1-10000</code>

2. **<code>T0 to 5</code> can be used but <code>T2, T3, T4</code> can show the best information because it can scan faster <code>T0</code> means it will scan very slowly and <code>T5</code> it is better not to use it because it can scan faster. Because of that many information can't show** > <code>nmap ip -p 1-1000 T0</code><br/>
3. **To scan a specific port** <code>nmap -p 445 ip -v</code>

4. **Checking with <code>-sV</code> will show what <code>Android, Mac, Windows, and Linux</code> he uses and what version they are.** > <code>nmap -p 445 ip -sV -v</code>

5. **If you use <code>-A</code>, you can create many pressure and bring information** > <code>nmap -p ip -A -v </code>

6. **<code>-O</code>scans inside the signature and shows what my target is using <code>Android Mac Linux Windows</code> but sometimes the information can be wrong** > <code>sudo nmap -p 1-1000 -O -v</code>

7. **script for dos attack ** > <code>ls /use/share/nmap/scripts | grep dos</code>

8. **any file found for ** > <code>ls /use/share/nmap/scripts | grep sh</code>


# Rustscan
### rustscan tool can scan very fast but sometimes does not show information properly due to scanning distance
1. **help for** > <code>rustscan -h</code>
2. **scan for ** > <code>rustscan -a ip -r 1-10000</code>


# Nbtscan
1. **one ip scan** > <code>nbtscan ip</code>
2. **lot ip scan** > <code>nbtscan -f filename</code>

# msfconsole 
1. **If you want to do enumeration with ssh or something else** > <code>nmap -p 1-1000 </code> **all ssh file show**
2. **exploit-module > <code>excellent, great, and good</code> to be good because while hacking the system this code destroys the system module code or breaks the system code and adds these codes there.**

3. **search any type module** > <code>search ssh type: auxiliary</code>

4. **if you any file select** > <code>use 20 </code> **module number**
5. **all details show** > <code>info</code>
6. **rhost change for** > <code>set rhost ip</code>
7. **check for** > <code>options</code>


8. **rport change for** > <code>set rports port-number</code>
9. **threads change** > <code>set threads 50</code> **Using this will allow the device to use CPU and send more packets and work faster**

10. **module run for** > <code>run</code> 
11. **back for** > <code>back</code>

12. **website or computer** > <code>ssh name@ip</code>
13. **Will show weakness** > <code>ssh-audit ip</code>
14. **Allows control of any device** > <code>ssh-remote</code>
15. **show details** > <code>search ftp type:</code><code>sudo cat /etc/resolv.conf</code><code>sudo cat /etc/hosts</code>



# dnsrecon 

1. **If dnsrecon is public it will try to pull it** > <code>dnsrecon -d xyz.com/ip</code>
2. **This will copy and show all records in this domain** <code>dnsrecon -d xyz.com/ip -t axfr</code>


