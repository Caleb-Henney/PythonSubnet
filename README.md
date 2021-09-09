# Python Subnet Calculator

A Python bot that tells a user-given IP address's network address, address range, broadcast, and next address in line
also prompt for subnet mask in slash notation, eg: /24
subnets have to be between 0 and 31
IP decimal octets must be between 0 and 255
store answers in sqlite3 database for later access to check answers
create its own inputs if errors occur or if the code is attempted to be broken
use https://subnetipv4.com/ to test answers.
The website isn't always perfect, though, so those I needed to double check I wrote by hand

## This code will
1. Ask the user for an IP address (write its own IP address if the user attempts to enter incorrectly)
2. Ask for a subnet mask (will make its own, similar to 1.)
3. Calculates Network address, First Host address, Last Host address, Broadcast address, and the Next subnet
4. Store calculated values in a database for withdrawal in case a repeated ip address is entered

### Example
```python
enter an IP address in this format: 'xxx.xxx.xxx.xxx': 234.148.112.157
Please enter a subnet mask: /28
Network Address:            234.148.112.144
First Host Address:         234.148.112.145
Last Host Address:          234.148.112.158
Broadcast Address:          234.148.112.159
Next Subnet:                234.148.112.160
```
