# cpu_load
Bash script to monitor the CPU and memory utilization of distributed Linux machines

In order to run this script without repeated password entries you need to set up an ssh key to store your password.
If not set up correctly, you'll need to enter your password for every single time you ssh to a machine
For setting up the ssh key look here: http://www.linuxproblem.org/art_9.html

If this script does not execute on your machine run: chmod 755 CPUload

The outut indicates the load over the last 1, 5 and 15 minutes as well as the memory usage
- a value of 1 means that the CPU is completely used
- a value greater than 1 indicates that there are other tasks waiting in line to execute
- a value smaller than 1 indicates free computational resources

To setup your machines to be monitored, open the script and replace "NameX" after "getLoad" with the name of the machine. Have one line for each machine.

