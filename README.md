# Operating-Systems-Project-1
Files for Operating Systems Project 1
This code produces the string "HelloWorld!" in a table with two parts, and then consumes it via shared memory.
To run the code, use:

gcc producer.cpp -pthread -lrt -o producer
gcc consumer.cpp -pthread -lrt -o consumer
./producer & ./consumer &

in the terminal.
