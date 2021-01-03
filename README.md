# udp_sum
A UDP server that returns the sum of all the integer numbers received since the last read. Specifically, the server receives one integer number at each read-from-socket operation, sums that number to the other numbers received until that, and sends the sum back to the client. When the number of received integers is equal to max_num_to_add, the sum is reset to 0. The program terminates when the client sends the string “exit\n” (with netcat you just need to digit the string exit and press enter).

# Running the code
You can run the test binary (which is called udp-sum) and send numbers using netcat (nc -u 127.0.0.1 55555). 
