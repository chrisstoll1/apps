# iSponsorBlockTV

[iSponsorBlockTV](https://github.com/dmunozv04/iSponsorBlockTV) skips SponsorBlock
segments on YouTube TV clients. This app uses the
[Web UI fork](https://github.com/chrisstoll1/iSponsorBlockTV) for browser-based
pairing, configuration, channel whitelists, and configuration import/export.

Open the Web UI and sign in using the username and password chosen during
installation. On the TV, open YouTube Settings, select Link with TV code, enter
that code in the dashboard, and save. A YouTube API key is only required for
channel whitelisting. Offline or unpaired TVs do not make the app unhealthy.

The worker and dashboard share persistent configuration at /app/data/config.json.
An existing configuration is preserved. For Host Path storage, grant the selected
user/group read and write access to the directory and existing config file.
Use HTTPS through a reverse proxy when accessing the dashboard over an untrusted
network. TV-code pairing requires no host networking or Docker socket access.
