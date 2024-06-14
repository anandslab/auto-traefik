<h3>Releases</h3>

<h5>June 15, 2024</h5>
<ul>
<li>NEW: Goodbye Auto-Traefik. Hello Deployarr - https://github.com/anandslab/deployarr</li>
<li>v3.3.3 will be the last version of Auto-Traefik.</li>
</ul>

<h5>v3.3.3 - June 6, 2024</h5>
<ul>
<li>NEW APPS: Nextcloud (not AIO version; uses existing Redis and MariaDB services), SABnzbd.</li>
<li>NEW: Graphics card detection (EXPERIMENTAL).</li>
<li>FIX: Traefik staging was failing while checking for staging certificates.</li>
<li>Other minor bug fixes.</li>
</ul>

<h5>v3.3.2.1 - May 27, 2024</h5>
<ul>
<li>FIX: Adding external app behind Traefik was broken.</li>
</ul>

<h5>v3.3.2 - May 25, 2024</h5>
<ul>
<li>NEW: ShellInaBox added (web-based terminal).</li>
<li>NEW: Authelia upgraded to v4.38.8.</li>
<li>NEW: Ability to set custom Docker folder and Backup folder.</li>
<li>ENHANCEMENT: UI/UX improvements throughout, including a new Apps menu.</li>
<li>ENHANCEMENT: More clarity on which steps are required and which ones are not.</li>
</ul>

<h5>v3.3.1 - May 23, 2024</h5>
<ul>
<li>NEW: Adminer, PostgreSQL, and Redis</li>
<li>NEW: Ability to create MariaDB database using the script (from Tools menu).</li>
<li>NEW: System Prep menu expanded with additional settings in preparation for future apps. Many of these are optional for now: SMTP Details, Downloads Folder, Media Folders, Server LAN IP, etc.</li>
<li>NEW: Ability to set a Traefik Auth Bypass Key - in preparation for future apps.</li>
<li>ENHANCEMENT: Reverse Proxy menu improved with more context based information (e.g. Number of external apps behind Traefik).</li>
<li>ENHANCEMENT: All sensitive info use by the script are now more securely stored as docker secrets.</li>
<li>ENHANCEMENT: Apps menu now shows status (Running), image version if available, and authentication mode beside their name.</li>
<li>ENHANCEMENT: Backups menu now shows the Backup Folder, Number of Backups, and Size of Backups Folder.</li>
<li>FIX: Ability to set authentication mode while added external apps behind Traefik was broken.</li>
<li>Several other minor fixes and improvements.</li>
</ul>

<h5>v3.3 - May 18, 2024</h5>
<ul>
<li>ENHANCEMENT: Colors galore! Color coding of menu and status texts for better UX.</li>
<li>NEW: Traefik v3 now default.</li>
<li>NEW: Traefik v2 to v3 migration assistant (EXPERIMENTAL).</li>
<li>NEW: Traefik Access and Errors now available via Dozzle.</li>
<li>FIX: With no Authelia and with OAuth, setting authentication system during app install wasn't working properly.</li>
<li>FIX: Rules syntax changes for Traefik v3 compliance.</li>
<li>FIX: Bash Aliases Fix - was erroring out previously.</li>
<li>Several other minor fixes and improvements.</li>
</ul>

<h5>v3.2.2 - April 26, 2024</h5>
<ul>
<li>NEW: New Name for Auto-Traefik: Deployarr (coming soon).</li>
</ul>

<h5>v3.2.1 - April 26, 2024</h5>
<ul>
<li>NEW: Speedtest-Tracker added.</li>
<li>FIX: Enabling authentication during app install was not working as expected.</li>
<li>OTHER: Additional minor bug fixes.</li>
</ul>

<h5>v3.2 - April 25, 2024</h5>
<ul>
<li>ANNOUNCEMENT: Auto-Traefik will be renamed shortly: "Traefik" is a trademarked word and Auto-Traefik does more than just Traefik.</li>
<li>ANNOUNCEMENT: Membership plugin that supports license verification will need an upgrade in the coming days. Please expect some down times that might hinder license checks.</li>
<li>NEW: Reverted a change introduced in 3.1. Sudoing should not be used when calling the script initially. Elevation to root will still be required after the script starts running.</li>
<li>NEW: Added Google OAuth (Traefik Forward Authentication).</li>
<li>NeW: Added Visual Studio Code Server (VS Code), DDNS Updater, and IT Tools.</li>
<li>NEW: Tools menu with Stack Manager, Backups, and Permissions Checks.</li>
<li>FIX: Improve Docker Folder permissions.</li>
<li>ENHANCEMENT: Improved service delete option to remove secrets as well.</li>
<li>ENHANCEMENT: Improved Auto-Traefik reset option.</li>
<li>ENHANCEMENT: Arranged all apps in alphabetical order in Apps menu.</li>
<li>ENHANCEMENT: Improved required info section with option to create new Linux users and warnings for certain situations (running as root, user not present, etc.).</li>
<li>Others: Over 2000 lines of code changed/improved.</li>
</ul>

<h5>v3.1.1 - April 16, 2024</h5>
<ul>
<li>NEW: Grafana added.</li>
<li>FIX: Prometheus permissions error.</li>
<li>ENHANCEMENT: Automated Vaultwarden Admin Token setup.</li>
</ul>

<h5>v3.1 - April 14, 2024</h5>
<ul>
<li>NEW: Sudo will now be required to invoke the script.</li>
<li>NEW: Stack Manager - Stop/Stop containers, Containers Status, Disable/Enable/Delete Services, and more.</li>
<li>NEW: Migrate and Restore Auto-Traefik and Docker Environment to a new system.</li>
<li>NEW: 'About' menu with relevant info on Auto-Traefik.</li>
<li>NEW: Added Glances.</li>
<li>NEW: Added Homarr.</li>
<li>NEW: Added InfluxDB.</li>
<li>NEW: Added Prometheus.</li>
<li>NEW: Added Vaultwarden.</li>
<li>NEW: Second domain passthrough to another Traefik instance on a different host, as explained in https://www.smarthomebeginner.com/multiple-traefik-instances/.</li>
<li>ENHANCEMENT: Improved compatibility with GLIBC. The script should now work on older version of Ubuntu/Debian/OMV.</li>
<li>ENHANCEMENT: Code improvements.</li>
<li>ENHANCEMENT: 'Authentication' Menu is now 'Security'.</li>
</ul>

<h5>v3.0.4 - March 29, 2024</h5>
<ul>
<li>ENHANCEMENT: Improved reliability of status/completion checks for various steps.</li>
<li>ENHANCEMENT: Reorganized menu to allow for future additions.</li>
<li>NEW: Added changelog view: Settings->View Changelog.</li>
</ul>

<h5>v3.0.3 - March 28, 2024</h5>
<ul>
<li>FIX: Removed compres middleware. Probably not important for homelab/low-traffic environment. Plus, this was causing "mine: no media type" error in Traefik logs.</li>
<li>ENHANCEMENT: Improved reliability of Docker Root Folder backups.</li>
<li>ENHANCEMENT: Added UDM/OPNsense specific troubleshooting tips.</li>
</ul>

<h5>v3.0.2 - March 21, 2024</h5>
<ul>
<li>FIX: Guacamole secrets error.</li>
<li>NEW: Automatic script updates - bye bye manual downloads!.</li>
<li>NEW: Ability to submit your rating/feedback.</li>
</ul>


<h5>v3.0.1 - March 18, 2024</h5>
<ul>
<li>FIX: Traefik dashboard 404.</li>
</ul>

<h5>v3.0 - March 15, 2024</h5>
<ul>
<li>NEW: Added Guacamole for Remote Admin</li>
<li>NEW: Backups (create, view, restore, and delete)</li>
<li>NEW: Additional ability (Docker Environment Setup, Socket Proxy Setup, etc.) for registered free-membership tier.</li>
<li>ENHANCEMENT: Added ability to set subdomain name during app setup</li>
<li>ENHANCEMENT: Added ability to set authentication type during app setup</li>
<li>ENHANCEMENT: Added feedback message when requirements are not met for a specific step</li>
<li>ENHANCEMENT: Authelia middlewares and configuration change to align with developer's recommendation</li>
<li>ENHANCEMENT: UI Improvements</li>
<li>ENHANCEMENT: Added password suggestions wherever password needs to be set</li>
<li>ENHANCEMENT: Added expert override for certain DNS issues</li>
<li>FIX: Bug fix for Docker Aliases</li>
</ul>
Over 1000 lines of code changed. 

<h5>v2.4.2 - February 27, 2024</h5>
<ul>
<li>Improved Traefik port 80 and 443 check for Traefik.</li>
<li>Implemented <a href="https://github.com/chaifeng/ufw-docker">UFW-Docker</a>. All though this appears to work, at this point it is an Experimental feature.</li>
<li>Implemented Docker secrets. At this point, this only applies to Traefik, Authelia, and MariaDB. This will be the default moving forward.</li>
<li>Improved the reliability of creating Docker secrets.</li>
<li>Added the ability to change authentication method for external/non-docker apps.</li>
<li>UI improvements for changing authentication methods for apps.</li>
<li>Changed Authelia users_database.yml to users.yml to align with Docs and <a href="https://www.smarthomebeginner.com/authelia-docker-compose-guide-2024/">Authelia guide</a> on SmartHomeBeginner.com</li>
</ul>

<h5>v2.4.1 - February 4, 2024</h5>
<ul>
<li>Bug fixes.</li>
</ul>

<h5>v2.4 - February 4, 2024</h5>
<ul>
<li>Unfortunately, many breaking changes, which make it incompatible with setup done with previous versions of the script.</li>
<li>Replace Cloudflare Email + Global API Key with Scoped API Token (CF_DNS_API_TOKEN)</li>
<li>Added Secrets for Basic HTTP Auth and CF_DNS_API_TOKEN</li>
<li>Additional Traefik checks - dangling TXT records, DNS error.</li>
<li>Improved port checks and added override option. </li>
<li>Changed DOMAINNAME variable to DOMAINNAME_1.</li>
<li>Docker Compose File now has the server's hostname as suffix.</li>
<li>Changed Traefik entrypoint names form http and https to web and websecure as in some online documentation.</li>
<li>Broke up middlewares to individual file providers instead of one middlewares.yml and middlewares-chain.yml</li>
<li>Added ability to put external apps behind Traefik.</li>
<li>Added MariaDB and phpMyAdmin.</li>
</ul>

<h5>v2.3.1 - January 5, 2024</h5>
<ul>
<li>Added override for port checks.</li>
</ul>

<h5>v2.3 - December 28, 2023</h5>
<ul>
<li>Simplified data entry forms.</li>
<li>Broke down and reassigned "Required Information" collection to their relevant section/steps instead of collecting all info at the beginning.</li>
<li>Added UI, instead of commandline for certain steps (e.g. Must Read Info, Authelia, etc.)
<li>Added Docker data size on disk and option to prune unused data/volumes/images.</li>
<li>Added option to uninstall/remove Auto-Traefik.</li>
<li>Added "Expert Mode" - will allow overriding certain steps (e.g. IP checks). Mode can be changed from Auto-Traefik Options.</li>
<li>Added Docker and Docker Compose version info to Docker menu.</li>
</ul>

<h5>v2.2.1 - December 6, 2023</h5>
<ul>
<li>Fix for the script not creating docker folders when they do not already exist.</li>
<li>Added comment on how to find Authelia verification email.</li>
</ul>

<h5>v2.2 - December 2, 2023</h5>
<ul>
<li>Potential fix for "Could not read certificate" error. Replaced openssl certificate check with acme.json file checks.</li>
<li>Removed unnecessary stoppage and restart of containers - only services being worked on will restart instead of the whole stack.</li>
<li>Improved the UI/UX for collecting required information and license check. </li>
</ul>

<h5>v2.1 - November 28, 2023</h5>
<ul>
<li>Several improvements and bug fixes. Potential fix for "Could not read certificate" error.</li>
<li>Added Dozzle, Homepage, and Uptime Kuma.</li>
</ul>

<h5>v2.0 - November 15, 2023</h5>
<ul>
<li>Free options for everyone - The system, docker, and port checks are available for anyone to use. No purchase necessary. This is great for anyone that wants to troubleshoot or to ensure that you system passes all checks to setup a Docker/Traefik stack.</li>
<li>Auto-Traefik now has 3 levels of licensing: Free/Unregistered, Auto-Traefik, and Auto-Traefik+ to fit the needs of most people.</li>
<li>Most of the navigation is now through a commandline GUI. This will continue to evolve.</li>
<li>Added ability to complete the whole process in steps, instead of one-go as in v1.</li>
<li>Expanded Auto-Traefik Options - reset, view key information, license checks, and build a sanitized troubleshooting log without any sensitive information.</li>
<li>Modified main docker compose file to now be more modular. All the individual services are available as individual yml files in a separate folder.</li>
<li>Added Authelia for multifactor authentication, with ability to change authentication mechanisms for apps from the UI.</li>
<li>Added Portainer. This is just the start. Many more apps will be added. </li>
<li>More to come.</li>
</ul>

<h5>v1.1.4 - October 31, 2023</h5>
<ul>
<li>Increased service start check timeout to avoid false positives</li>
</ul>

<h5>v1.1.3 - October 30, 2023</h5>
<ul>
<li>Minor changes to logging - added a few more logging spots</li>
<li>Updated Traefik version to 2.10</li>
<li>Fixed a bug where subdomain resolution check would not exit on error</li>
</ul>

<h5>v1.1.2 - October 16, 2023</h5>
<ul>
<li>Added auto-traefik output logging to /tmp/auto-traefik/auto-traefik.log to help troubleshoot</li>
<li>Added failsafe - in case container with same name already exists, script will fail</li>
</ul>

<h5>v1.1.1 - October 14, 2023</h5>
<ul>
<li>Added a backup method to check WAN IP. Some IP check sites present Cloudflare challenge, interfering with the process.</li>
</ul>

<h5>v1.1 - October 9, 2023</h5>
<ul>
<li>Added version check. Now the users will see a warning of there is a new version available for download.</li>
<li>Clean up repository and organized files.</li>
<li>Reduced unnecessary sleeps/waits in the script.</li>
<li>Improved check for certificates, instead of sleeping for a certain time, which can fail sometimes. </li>
<li>Added check for Let's Encrypt rate limiting.</li>
<li>Added backup for acme.json if successful. Can be handy if rate limit is hit.</li>
</ul>

<h5>v1.0 - September 23, 2023</h5>
<ul>
<li>Initial Release</li>
</ul>