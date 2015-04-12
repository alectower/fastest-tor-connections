# Fastest Tor Connections

This is a ruby script to find ip addresses for the fastest connection to tor servers within a certain country. Results are based on ping results from a specified ip address.

# Requirements

* Ruby
* Ruby Gems - HTTParty, net-ping

# Usage

```
fth <country symbol> <ip address> [number of results]
```

# Examples
Retrieve 5 US ip addresses of tor servers with the fastest connections based on ping results from 123.456.78.9 (Use your external router ip address)
```
fth us 123.456.78.9 5
```
