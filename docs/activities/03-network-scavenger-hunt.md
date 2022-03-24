# Network Scavenger Hunt

The goal of this activity is to learn to find out how your computer is connected to the internet.

## Step 1: What is My IP Address?

Each computer on the internet is assigned its own Internet Protocol Address.  What is the address assigned to your computer?  (Hint: use a search to find a service that tells you what your IP address is)

## Step 2: What is the name of your WiFi Network

Each computer that uses WiFi must connect to the network through a WiFi router that has a name?  How can you find out what your WiFi network name is?
(Hint: use a search service to find the instructions for your device: Chrome, Windows, Mac, iPad)

## Step 3: How fast is your connection?

Look for a program that can test your connection speed.  What is your download and upload speed?

## Advanced Labs

To do these labs, you will need to access your computer's command shell or Terminal (on the Mac).

### Ping Test Lab

Ping is a useful program that will help you see the time it takes your computer to communicate with a report computer.  It is named after the way that submarines sent out sounds underwater to see what items were near it (sonar).  You can use it to debug network problems.

Search for how to use the "ping" program on your operating systems:

* **How do I run ping on Windows 10"**
* **How do I run ping on a Mac"**
* **How to run a ping test in Chrome OS** (requires ChromOS Shell crosh) [Video](https://www.youtube.com/watch?v=WOIeXlHPoPc) - your school may not have crosh enabled.

For example on the Mac use the Terminal and type "ping -c 10 google.com".  This will measure the time to get from your computer to google.com with a "count" of 10.

```
$ ping -c 10 google.com
PING google.com (142.250.191.142): 56 data bytes
64 bytes from 142.250.191.142: icmp_seq=0 ttl=50 time=47.229 ms
64 bytes from 142.250.191.142: icmp_seq=1 ttl=50 time=52.301 ms
64 bytes from 142.250.191.142: icmp_seq=2 ttl=50 time=43.634 ms
64 bytes from 142.250.191.142: icmp_seq=3 ttl=50 time=51.289 ms
64 bytes from 142.250.191.142: icmp_seq=4 ttl=50 time=51.612 ms
64 bytes from 142.250.191.142: icmp_seq=5 ttl=50 time=51.738 ms
64 bytes from 142.250.191.142: icmp_seq=6 ttl=50 time=48.213 ms
64 bytes from 142.250.191.142: icmp_seq=7 ttl=50 time=46.793 ms
64 bytes from 142.250.191.142: icmp_seq=8 ttl=50 time=56.455 ms
64 bytes from 142.250.191.142: icmp_seq=9 ttl=50 time=52.937 ms

--- google.com ping statistics ---
10 packets transmitted, 10 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 43.634/50.220/56.455/3.522 ms
```

The last column in the list is the time it took to make a round trip in milliseconds.  At the end of the test it will show you the minimum, average, maximum and standard deviation of the 10 trials.  The average of 50.22 is a reasonable number.  This is about 1/20th of a second.

Questions:

1. Why do you think there are variations in the times?
2. What do you think happens if one of the computers connecting your computers goes down? (crashes)