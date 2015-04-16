# Fastest Tor Connections

This is a ruby script to find ip addresses for the fastest connections to tor servers within a certain country. Results are based on ping results from a specified ip address.

# Requirements

* Ruby
* Ruby Gems - HTTParty, net-ping

# Usage

```
ftc <country symbol> <ip address> [number of results]
```

# Examples
Retrieve 5 US ip addresses of tor servers with the fastest connections based on ping results from 123.456.78.9 (Use your external router ip address http://whatismyipaddress.com)
```
ftc us 123.456.78.9 5
```

# Limitations

* Country information for ip addresses is retrieved through http://ipinfo.io which has a request limit of 1000/day
* Some ips gathered from https://check.torproject.org/cgi-bin/TorBulkExitList.py?ip=<ip> don't work when added to .torrc, even after getting successful ping response
