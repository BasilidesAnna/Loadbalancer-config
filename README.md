# Load Balancer configuration

In this project a very simple nginx load balancer configuration forwards requests to webservers, also hosted by nginx, on localhost:8081 !!

The webservers and the loadbalancer also running in Docker container.

If you run the vagrant virtual machine, it will take some time until everything stand up, after that if you cURL localhost the loadbalancer will always forward you a different server (in the config file there is round robin type loadbalance, becouse the type is not defined).

!!Load balancing may not work, if you would like to see it in browser, it's because of the cache. If you use Ctrl+F5 and Ctrl+R alternately in Chrome, you can see that nginx gives you different servers.!!

**Base requirements:**

 - git (https://git-scm.com/downloads)
 - Vagrant (https://www.vagrantup.com/downloads)
 - Virtualbox (https://www.virtualbox.org/wiki/Downloads)
