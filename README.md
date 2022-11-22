## fake-traffic

fake-traffic [road warrior](http://en.wikipedia.org/wiki/Road_warrior_%28computing%29) installer for Ubuntu, Debian, AlmaLinux, Rocky Linux, CentOS and Fedora.

---
### Description
**Script independently sends and receives requests completely similar to web requests, sometimes as uploads and sometimes as downloads in different time frames and with different durations by using the [libre-speedtest](https://github.com/librespeed/speedtest-cli) package.**

---
### Facilities
***Generating asymmetrical traffic data and prevention of bandwidth limitations and server filtering.***

---

### Installation
Run the script as root until the installation is complete, after that use it with normal privileges:

`curl -L short.platonic.ir/ft -o fake-traffic && bash fake-traffic`

---

### Run Every 3 hours

 `{ crontab -l; echo "0 */3 * * * fake-traffic &>> ~/.fake-traffic.log"; } | crontab -`

---

### Logs can also be checked from this path:

`cat ~/.fake-traffic.log`
