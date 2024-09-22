# 42_born2beroot

The goal of this project is to familiarize with basic system administration skills. It entails the creation of a virtual machine using VirtualBox and set up an operating system with a set of specific security and configuration guidelines.

## Mandatory Part

#### Virtual Machine Setup:</br>
  - Use either the latest stable version of Debian or Rocky Linux. Debian is recommended for beginners.</br>
  - Install a minimum of services. A graphical interface is not allowed.

#### Server Configuration:</br>
  - Create at least 2 encrypted partitions using LVM.</br>
  - Set up a SSH service running on port 4242. Root login via SSH should be disabled.</br>
    - Implement a strong password policy:</br>
      - Passwords must expire every 30 days.</br>
      - Minimum of 10 characters with at least one uppercase letter, one lowercase letter, and a number.</br>
      - No more than 3 consecutive identical characters.</br>
    - Configure sudo with the following rules:</br>
      - Limit to 3 attempts for authentication.</br>
      - Display a custom error message on incorrect password.</br>
      - Archive each action using sudo.</br>

#### Monitoring Script:
  - Develop a monitoring.sh script in bash.
  - Display system information every 10 minutes on all terminals using the wall command.
    - Information to display includes:
      - OS architecture and kernel version.
      - CPU and memory usage.
      - Disk usage.
      - Active connections.
      - IPv4 and MAC addresses.

## Bonus Part
To earn bonus points, you can set up additional services or improve your system configuration:
  - Configuring a functional WordPress website with Lighttpd, MariaDB, and PHP.
  - Setting up any other useful service of your choice (excluding NGINX/Apache2) I included an FTP service.
