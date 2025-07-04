# TASK-8-CYBER-SECURITY-INTERSHIP-
# Task 8: Configuring and Using a VPN on Windows 11

**Introduction:** Virtual Private Networks (VPNs) create a secure “tunnel” between your device and the internet.  When active, a VPN routes all your traffic through a remote server, encrypting it and hiding your real IP address.  For example, we used the UrbanVPN Windows client to connect through a server in Germany.  After connection, our public IP appeared to be in Germany (not our true location), confirming the VPN had hidden our real IP.  By encrypting traffic and assigning a new IP from the VPN server, a VPN makes it appear as though you are browsing from the server’s location.  This enhances privacy: websites and ISPs see only the VPN’s IP, not yours, so your identity and activity are obscured.

UrbanVPN on Windows 11 encrypts your traffic and replaces your IP with the VPN server’s IP, hiding your real location.  In other words, **all websites and networks see the VPN’s IP and encrypted data instead of your real IP**.  This protects your identity and browsing activity from being easily traced back to you.

## Installing UrbanVPN on Windows 11

To install UrbanVPN on Windows 11, follow these steps:

* **Step 1:** Open the **Microsoft Store** and search for “UrbanVPN”. Click **Get** (or **Install**) to download the official app.  (Alternatively, go to the official UrbanVPN website and download the Windows installer.) This ensures you get a legitimate, untampered client.
* **Step 2:** Once downloaded, **launch UrbanVPN**. You may be prompted to grant permissions—allow them. The UrbanVPN icon will appear in the Windows system tray (bottom-right on the taskbar).
* **Step 3:** Click or right-click the **UrbanVPN tray icon** to open its menu. You should see a list of server locations (countries). At this point the app is ready for connection.

Each step above takes only a moment. Once installed and launched, UrbanVPN is ready to connect to a remote server.

## Connecting to a VPN Server

With UrbanVPN running, you must select a server location and connect.  Follow these steps:

* **Select a location:** In the UrbanVPN menu, choose **Germany** (or your desired country) from the server list.  This tells the app to route your traffic through a German IP address.
* **Connect:** Click the **Connect** button (or simply ensure the Germany server is highlighted). The UrbanVPN icon will change or animate, indicating an active connection. Wait a few seconds for it to establish.
* **Confirmation:** Once connected, all your internet traffic is routed through the German server. At this point your **real IP is replaced by a German IP**. UrbanVPN on Windows uses the OpenVPN protocol, which provides strong security and speed.

After connecting, UrbanVPN shows that you are online through the German server. All data between your PC and the VPN server is now encrypted via the OpenVPN tunnel.

## Verifying the IP Address Change

To confirm that the VPN is working, you can check your public IP before and after connecting:

1. **Check original IP:** Disconnect UrbanVPN (turn it off). Open a browser and go to an IP-check site such as *WhatIsMyIPAddress.com*. Note the IP address and the shown location; it should reflect your real location.
2. **Enable the VPN:** Re-open UrbanVPN and connect to the Germany server. After a few seconds, return to the IP-check site and refresh the page.
3. **Compare results:** The site should now display an IP address in Germany. In other words, your public IP has changed to a German one provided by UrbanVPN.  Seeing a different country and IP confirms the VPN is active and masking your real IP. If the IP did not change, try disconnecting and reconnecting or picking another server. By definition, a working VPN hides your true IP.

*Example:* Before VPN, the site might show “United States, IP 203.x.x.x.” After connecting to Germany, it should show “Germany, IP 85.x.x.x.” The mismatch confirms success. (Do **not** share actual IPs; just verify that the location changed to the VPN country.)

## How a VPN Masks Your IP and Enhances Privacy

A VPN protects you in two main ways:

* **IP Masking:** When connected, UrbanVPN replaces your device’s IP address with one from the VPN server.  For instance, selecting Germany gives you a German IP. All websites and network services see this VPN IP instead of your real IP.  This hides your true location and identity.  Outsiders (websites, advertisers, or your ISP) cannot link your activity to your real IP or location.  In short, **your real IP is shielded by the VPN server’s IP**.
* **Encryption:** UrbanVPN uses the OpenVPN protocol on Windows, which creates a secure, encrypted tunnel for all your data.  Even if someone intercepts your connection (e.g. on public Wi-Fi), they see only encrypted gibberish. Only your computer and the VPN server hold the decryption key.  As Kaspersky explains, **all your data traffic is sent through an encrypted virtual tunnel**. This means logins, passwords, and browsing data remain private.  In effect, **anyone snooping on the network can’t read your data or link it to you**.

Together, IP masking and encryption mean that observers (like ISPs, Wi‑Fi providers, or websites) see only the VPN server’s IP and encrypted traffic. Your actual IP, location, and content are hidden. The VPN makes it appear as if you are browsing from the VPN server (Germany in our case), keeping your true identity and activity private.

## Task Summary

In this task we performed the following on Windows 11:

* **Downloaded and installed** the official UrbanVPN Windows app.
* **Launched UrbanVPN** and opened its system-tray icon to view server options.
* **Selected Germany** as the VPN server and clicked **Connect**, establishing an encrypted tunnel.
* **Verified the IP change:** An external IP-check site showed a German IP after connecting (versus our original IP without VPN), confirming our real IP was successfully masked.

These steps demonstrate how to set up and use UrbanVPN on Windows 11 to protect your privacy and appear online from the VPN’s location.

## Best Practices for Safe VPN Use

When using any VPN, follow these guidelines for maximum security:

* **Download official software:** Always get the VPN app from a trusted source (e.g. the Microsoft Store or UrbanVPN’s website). Avoid third-party downloads or torrents, which may be tampered with. Official versions are less likely to contain malware.
* **Keep software updated:** Install updates for UrbanVPN and Windows promptly. Updates often include security fixes that protect against new threats.
* **Use strong credentials:** Choose a unique, strong password for your VPN account. Enable two-factor authentication (2FA) if offered. This prevents attackers from easily hijacking your VPN account.
* **Understand limitations:** A VPN encrypts your connection, but it *does not* scan for viruses or block phishing sites. It won’t stop malware, nor replace good security software. Continue using antivirus/anti-malware protection and avoid suspicious links or downloads. In other words, don’t rely on the VPN alone to protect against all threats.
* **Enable a kill switch (if available):** Some VPNs include a “kill switch” feature that cuts off all internet traffic if the VPN drops unexpectedly. Enabling this prevents any data from leaking outside the VPN tunnel in case of a disconnection. Check UrbanVPN’s settings to use this feature if present.
* **Log out when idle:** Disconnect UrbanVPN and sign out of the app when you’re done, especially on shared or public computers. This ensures others can’t use your VPN session. Do not share your VPN login credentials.
* **Double-check your connection:** Periodically revisit an IP-check site to ensure your VPN is working as expected. It’s a good habit to confirm your IP and location remain the VPN’s rather than your real one.
