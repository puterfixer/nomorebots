# nomorebots
Banned IP subnets running abusive (brute force, spam) attack bots

This is a collection of IP subnets which were triggering the fail2ban repeatedly
on a web server I used to maintain through hammering the SSH or Wordpress' login.

As the websites were intended to be read by people, not by servers in datacenters,
I also had zero remorse to ban entire cloud providers and webhosts.

The list was relevant for the traffic *my* server and domains were attracting. You
might find it completely useless for your particular case.

Meanwhile the server has reached its end of life, the sites were moved to other
type of hosting, I changed the strategy for protecting the domains against
unwanted traffic, so the list is not maintained and will not receive updates.
I'm still leaving it here in case it does help anyone, at least for a couple years.

The more elegant solution is to funnel all traffic through Cloudflare. Most sites
will not exceed the limits for the free services tier, and the level of control
is far better than what could be achieved through a crude blacklisting of IP
subnets on your own software firewall. In Cloudflare you can ban entire AS numbers
with all the tens or hundreds of (dynamic) subnets in one go, you can ban TOR
proxies through a couple of clicks, it can also run its own bot detection with a
(momentarily better than Google's) captcha before traffic even reaches your server.

Good luck and stay safe.
