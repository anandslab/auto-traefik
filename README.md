# IMPORTANT: Auto-Traefik has moved!

Auto-Traefik is now called Deployarr: https://github.com/anandslab/deployarr

v3.3.3 will be the last version of Auto-Traefik. All future updates will be available via the Deployarr repository.

# What is Auto-traefik?
Automatically setup Socket Proxy, Traefik (fetch LE SSL certificates), Authelia, Portainer, Dozzle, Uptime-Kuma, Homepage, and other apps. 

<div class="announcement"><h5>Name Change Coming</h5><strong>Auto-Traefik</strong> will soon be renamed to <strong>Deployarr</strong> to accurately reflect what it does - simplify deployment of several Homelab apps, on top of Traefik.</div>

# Tested On
<ul>
<li>Ubuntu</li>
<li>Debian</li>
<li>May also work on OMV but not fully tested</li>
</ul>

<del>GLIBC version 2.35 needed (use the command below to check your system). Older versions of the above OSes tend to have older version of GLIBC. </del>

Since Auto-Traefik v3.1, most recent version of Ubuntu/Debian/OMV with older GLIBC versions should be supported.

# More Details
https://www.smarthomebeginner.com/auto-traefik/

# How to Use Auto Traefik? - Guides
## Text Guide 
https://www.smarthomebeginner.com/course/how-to-use-auto-traefik/

## Video Guide
### Playlist:
https://www.youtube.com/playlist?list=PL1Hno7tIbSWViTyCXl9xNdXXU-1bVxIFD

### Individual Videos:<br/>
1️⃣: Introduction, Version 2 Overview, and New Features: https://youtu.be/ePBLJTyRgdQ<br/>
2️⃣-3️⃣: Must Read Info and Checks: https://youtu.be/hF-Ip18Y4kc<br/>
4️⃣: Docker and Socket Proxy Setup: https://youtu.be/TWsLUzK6DbM<br/>
5️⃣: Traefik Staging and Production Setup: https://youtu.be/SBv-9LD1S5k<br/>
6️⃣: Authentication, Basic Auth, and Authelia MFA: https://youtu.be/1g9h9P3QYl8<br/>
7️⃣: Applications: https://youtu.be/RnoFPgwS534<br/>
8️⃣: Additional Applications: https://youtu.be/GK0YKA5q1XE<br/>
9️⃣: External Apps Behind Traefik: https://youtu.be/kGaX1pnP_y4<br/>
1️⃣0️⃣: Removing Auto-Traefik and Closing Thoughts: https://youtu.be/z9Az9MMBHSE<br/>

# Download Auto-Traefik
```
wget https://raw.githubusercontent.com/htpcBeginner/auto-traefik/main/auto-traefik_v3.3.3.shb
```
# Run the Bash Script
Once you have the script on the server, run it using the following commands (do not use ```sudo```):
```
chmod +x auto-traefik_v3.3.3.shb
./auto-traefik_v3.3.3.shb
```

Use the <strong>-arm.shb</strong> version of the file for Raspberry Pi. 

# Support
Please do not open issues on GitHub. There is a dedicated Auto-Traefik support channel on our [Discord server](https://www.smarthomebeginner.com/discord/) for Supporters.