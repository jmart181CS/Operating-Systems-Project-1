# Operating-Systems-Project-1
Files for Operating Systems Project 1
This code produces the string "HelloWorld!" in a table with two parts, and then consumes it via shared memory.
To run the code, use:

gcc producer.cpp -pthread -lrt -o producer
gcc consumer.cpp -pthread -lrt -o consumer
./producer & ./consumer &

in the terminal.

# Implementation:

While I was implementing this program, I encountered many problems that I had to rectify. The first of the problems began before I even started working on the project, as it was my first time using a Linux environment and a virtual machine. Getting the virtual machine operational came with a suprising amount of troubleshooting. It involved a trip to my computer's BIOS and some trial and error to get everything working. 
Then, I needed to learn how to use Linux for the first time. Due to my previous experience with Unix, this wasn't that much of an issue, but it was definately new to me. Finally, I needed to get a shared folder between my computer and the virtual machine, which took a couple attempts to get working. Including a unique bug where my shared folder on the virtual machine's end would be wiped clean each time I restarted the machine. 
After making sure there wasn't anything wrong with the virtual machine, I began working on the project. While working, I wanted to make sure I could get the program to run in just a singular file before moving to two files. This was to make sure I understood the actual concept of the producer-consumer problem. After that was operational, the next step was to implement the shared memory. I decided to do this by using the IPC Posix inter-program communication. This was hard to get operational, because the code was very new to me, and was initally hard to understand.
Eventually, I managed to understand how the code was communicating with eachother through the unique functions. However, while I was implementing the code, I ran into a few errors. The easiest bug that I fixed was package dependancies. I realized that I didn't have all the packages for the functions that I needed to use. The hardest part was tracking down the packages that I needed specifically.
Next, there was a bug that prevented the pointer from printing out the messages that I needed. After a little bit of troubleshooting, I found out that setting the pointer variable to char from void in the messsages that I needed solved my issue.
This project was very challenging with all of the new concepts that were being used in the project. Additionally, I personally had the added troubles of using a virtual machine and linux for the very first time. This project was a good crash course into the concepts of shared memory and the producer and consumer problem, as well as a good practical guide to linux and virtual machines.
