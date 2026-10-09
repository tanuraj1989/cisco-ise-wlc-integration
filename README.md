# cisco-ise-wlc-integration
Identity Access Management : Cisco ISE Integration with Cisco WLC for Guest Wi-Fi
This repository document has demonstrates how to integrate Cisco Identity Services Engine (ISE) with a Cisco Wireless LAN Controller (WLC) to implement Central Web Authentication (CWA). The setup enables secure guest access, BYOD onboarding, and centralized policy enforcement for wireless clients—ideal for enterprise and government organizations. I have completed this project in a government organization for almost 1000 users. The requirements were : i) Device Administration (Tacacs). ii) User Access (Radius). iii) Central Web Authentication for the guest users (Self-sign login)

📋 Overview
Cisco ISE acted as the RADIUS server and policy engine.
Cisco WLC for WLAN creation, client redirection, and VLAN/ACL, policy configuration.
Central Web Authentication provides a captive portal for guest self-registration and login.
🛠 Features
RADIUS server integration with shared secret synchronization.
Authorization Profiles:
GUEST_Redirect_ISE – Captive portal redirection.
Allow_Guest – Grants network access after authentication.
Policy Sets for guest Wi-Fi:
MAC Authentication Bypass (MAB) for pre-auth checks.
Authentication and Authorization policies for SSID-based access.
Guest Portal with:
Self-registration and temporary password issuance.
Forced password change on first login.
Cisco WLC configuration:
MAC filtering and VLAN mapping.
ACL creation for web redirection and post-auth traffic.
CoA (Change of Authorization) support for dynamic policy enforcement.
