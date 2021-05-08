---
title: "Role Studio"
permalink: /en/admin-studio
excerpt: "Role studio"
redirect_from:
  - /theme-setup/
---

{% include base_path %}
This user can login into the web UI and make calls to Journalists, Guest users, mobile or landline phone numbers and SIP Codecs

Select the role: "ROLE_STUDIO"

# Permissions

Configure permissions to access different options in the web UI

* Administrator, allows access to administration section
* Bitrate, user can override the bitrate for any call
* Configure alias, user can create alias for calls
* Can view stats, user can access the call statistics
* Temporal admin, user can create guest users
  * Temporal group, if Temporal admin is enabled, the group the user can admin
  
|![](/en/admin-studio/permissions.png)|  
|:--:|
|*Permissions*|

# Audio controls

In this section you can configure the different audio controls

* Max calls, the maximum number of simultaneous calls. This is defined by your license type
* On Air Groups, the number of On Air Groups that you will use in your Studio. Define this depending on your available resources in your PC and audio mixer
* Show all on air group, if enabled you all On Air buttons, up-to 10. If not enabled it shows On Air 1 and the second On Air can be configured with the right button
* Default bitrate, the bitrate that applies for every calls
* Push to talk, if enabled you need to keep pressed the Talk button
* Allow talk in on-air, it enables or disables talk button while the call is on-air
* Deactivate PFL with on-air, if enabled PFL will be automatically deactivated when you click in any on-air button
* Activate PFL with on-air, if enabled PFL will be automatically activated when you disable on-air button
* PFL listen on-air, if enabled any user that is not in On Air will listen to On Air 1 input

|![](/en/admin-studio/audio-controls.png)|
|:--:|
|*Audio controls*|

# Noise gate

Noise gate settings

* Enable noise gate, automatically enable noise gate in every call
* Configure noise gate, studio user can access the configuration of noise gate in live connections
* Thresdhold in DBFS that apply by default
* Attack time in seconds that apply by default
* Release time in seconds that apply by default

|![](/en/admin-studio/noise-gate.png)|
|:--:|
|*Noise gate settings*|

# SIP

SIP configuration. You can use the embedded SIP Server included with your license.

To use an external SIP Server it must comply with the SIP Over Websocket standard [The websocket Protocol as a Transport for the Session Initiation Protocol SIP RFC-7118](https://tools.ietf.org/html/rfc7118)

If you need to register your IP Codec please open a ticket with the support team

* SIP checkbox enables SIP Support
* SIP username
* SIP password
* Auto answer extension, any call from this extension to the studio will be automatically answered
* Auto reject, any call from any extension (except auto answer extension) will be automatically rejected
* Transfer extension, allows to transfer any call from the studio to this extension

|![](/en/admin-studio/sip.png)|
|:--:|
|*SIP configuration*|


