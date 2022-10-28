# Operating-Systems-Project-1
Files for Operating Systems Project 1
This code produces the string "HelloWorld!" in a table with two parts, and then consumes it via shared memory.
To run the code, use:

gcc producer.cpp -pthread -lrt -o producer
gcc consumer.cpp -pthread -lrt -o consumer
./producer & ./consumer &

in the terminal.

# Implementation:

While I was implementing this program, I encountered many problems that I had to rectify. The first of the problems began before I even started working on the project, as it was my first time using a Linux environment and a virtual machine. Getting the virtual machine operational came with a suprising amount of troubleshooting. It involved a trip to my computer's BIOS and some trial and error to get everything working. Then, I needed to learn how to use Linux for the first time. Due to my previous experience with Unix, this wasn't that much of an issue, but it was definately new to me. Finally, I needed to get a shared folder between my computer and the virtual machine, which took a couple attempts to get working. Including a unique bug where my shared folder on the virtual machine's end would be wiped clean each time I restarted the machine.
