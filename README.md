# SYN_Flood_Attack_using_Python

The code serves to execute a SYN Flood Attack on a Machine. If the SYN Cookie countermeasure is disabled (the attack will fail if it is enabled as it will verify if it received an ACK packet with a valid SYN cookie) and this code is executed you will not be able to establish a connection with the machine (for example by using telnet, i.e. <telnet {IP_address}>). The connection will time out.
