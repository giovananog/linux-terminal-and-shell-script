# Network/Service Configuration Commands

- `ifconfig` - Display or configure network interface parameters.
  - **Example:** `ifconfig`
  - This command, while commonly used in the past, has been deprecated on many modern Linux distributions. The recommended replacement is `ip`.

- `ip addr show` - Show information about network interfaces.
  - **Example:** `ip addr show`
  - This is the modern replacement for `ifconfig` and provides detailed information about all network interfaces.

- `ifconfig eth0 up` - Bring the Ethernet interface `eth0` up (activate).
  - **Example:** `ifconfig eth0 up`
  - Activates the specified network interface, allowing it to send and receive data.

- `ifconfig eth0 down` - Bring the Ethernet interface `eth0` down (deactivate).
  - **Example:** `ifconfig eth0 down`
  - Deactivates the specified network interface, stopping its ability to send or receive data.

- `ifconfig eth0 192.168.1.2` - Set the IP address of `eth0` to `192.168.1.2`.
  - **Example:** `ifconfig eth0 192.168.1.2`
  - Manually sets the IP address of the specified network interface.

- `ifconfig eth0 netmask 255.255.255.0` - Set the netmask of `eth0`.
  - **Example:** `ifconfig eth0 netmask 255.255.255.0`
  - Specifies the network mask associated with the IP address.

- `ifconfig eth0 hw ether 00:11:22:33:44:55` - Set the MAC address of `eth0`.
  - **Example:** `ifconfig eth0 hw ether 00:11:22:33:44:55`
  - Manually sets the hardware (MAC) address of the specified network interface.

- `route` - Display or configure the IP routing table.
  - **Example:** `route`
  - Shows the routing table, indicating the paths that network packets can take.

- `route add default gw 192.168.1.1` - Add a default gateway.
  - **Example:** `route add default gw 192.168.1.1`
  - Sets the default gateway for network traffic.

- `netstat -nr` - Display routing table information.
  - **Example:** `netstat -nr`
  - Provides a detailed view of the system's routing table.

- `traceroute` - Trace the route to a network host.
  - **Example:** `traceroute www.example.com`
  - Shows the route that packets take to reach a destination, indicating network delays.

- `ping` - Send ICMP ECHO_REQUEST to network hosts.
  - **Example:** `ping www.example.com`
  - Tests the reachability of a host on an Internet Protocol (IP) network.

- `service serviceName start` - Start a system service.
  - **Example:** `service apache2 start`
  - Initiates the specified service, in this case, starting the Apache web server.

- `service serviceName stop` - Stop a running system service.
  - **Example:** `service apache2 stop`
  - Halts the specified service, such as stopping the Apache web server.

- `service serviceName restart` - Restart a system service.
  - **Example:** `service apache2 restart`
  - Stops and then starts the specified service, often used after configuration changes.

- `service serviceName status` - Check the status of a system service.
  - **Example:** `service apache2 status`
  - Provides information about whether the specified service is running or stopped.