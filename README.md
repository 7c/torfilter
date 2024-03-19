# TORFilter
The TOR network's exit nodes are monitored and listed for abuse prevention reasons; this list will be updated hourly. The list is separated into 'last seen' groups. For example, 'torfilter-1d' contains all exit nodes that have been seen in the last 24 hours.


# Feed
We source our data from `https://www.dan.me.uk/tornodes`, `https://check.torproject.org/torbulkexitlist` (a TOR project feed), and from other automated research projects.

# Types
## flat
One IP (IPv4 or IPv6) per line.

## cidr
...coming soon...

IPv6 especially enables exit nodes to randomize outgoing IP addresses within the large subnets available to them. Since TOR does not expose those CIDRs, it's challenging to identify the networks available to TOR exit nodes.

# Formats
## txt format
Flat list of IP addresses.

## markdown format
Markdown version of same IP addresses list.

## json format
This format has more details about ip addresses:
```json
....
{
      "ip": "23.....100",
      "ipversion": 4,
      "firstseen": 1648437978,
      "lastseen": 1710594950,
      "countrycode": "..",
      "city": "N....",
      "ASN": 2x0xx,
      "rdns": "tor-exit....."
},
...
```

*Disclaimer:* We are not responsible for any damage caused by the use of this list. Use it at your own risk. We do not recommend outright banning based on this list alone. Instead, you may want to use this list to help classify incoming requests, packets, or registrations in your services.

