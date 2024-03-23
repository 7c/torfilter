# TORFilter
The TOR network's exit nodes are monitored and listed for abuse prevention reasons; this list will be updated hourly. The list is separated into 'last seen' groups. For example, 'torfilter-1d' contains all exit nodes that have been seen in the last 24 hours.


# Feed
We source our data from `https://www.dan.me.uk/tornodes`, `https://check.torproject.org/torbulkexitlist` (a TOR project feed), and from other automated research projects.

# Charts
we generate different charts about available data in this repo. For example `counts-1h` shows the number of IPs updated in the last hour. This means if you took this list as base you can see how many IPs you would have inside. 

![counts-1h](https://torfilter.com/img/chart-counts-1h.png)

![counts-6h](https://torfilter.com/img/chart-counts-6h.png)

![counts-1d](https://torfilter.com/img/chart-counts-1d.png)

![counts-1w](https://torfilter.com/img/chart-counts-1w.png)

# Types
## flat
One IP (IPv4 or IPv6) per line. (current)

## cidr
...coming soon...

IPv6 especially enables exit nodes to randomize outgoing IP addresses within the large subnets available to them. Since TOR does not expose those CIDRs, it's challenging to identify the networks available to TOR exit nodes.

# Formats
## txt format
Flat list of IP addresses. For example:

[torfilter-1h-flat](lists/txt/torfilter-1h-flat.txt)

## markdown format
Markdown version of same IP addresses list. For example:

[torfilter-1h-flat](lists/markdown/torfilter-1h-flat.md)



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
      "continentcode": "SA",
      "city": "N....",
      "ASN": 2x0xx,
      "rdns": "tor-exit....."
},
...
```

*Disclaimer:* We are not responsible for any damage caused by the use of this list. Use it at your own risk. We do not recommend outright banning based on this list alone. Instead, you may want to use this list to help classify incoming requests, packets, or registrations in your services.

