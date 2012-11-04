# Simple Bouncer (TCP)

Inspired in [rinetd](http://www.boutell.com/rinetd/) and [stunnel](https://www.stunnel.org/static/stunnel.html) this bouncer is Java-minimalistic version.

SimpleBouncer is an open source (Apache License, Version 2.0) Java application.

## Config (bouncer.conf)

    # <bind-addr> <bind-port> <remote-addr> <remote-port> [options]
    0.0.0.0 1234 127.1.2.3 9876
 
 * Options are comma separated:
  * **LB=ORDER**: active failover-only in DNS order
  * **LB=RR**: active LoadBalancing in DNS order (round-robin)
  * **LB=RAND**: activate LoadBalancing in DNS random order
  * **TUN=SSL**: activate SSL tunneling (origin is plain, destination is SSL)


