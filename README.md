# Github notifications

[![Connect IQ(R)](https://github.com/eternal-flame-AD/git-notifications-ciq/blob/master/docs/img/connect-iq-logo-white.png?raw=true)](https://apps.garmin.com/en-US/apps/7debce23-b6ec-48f5-b902-9cfdeaaab5d2)

## Screenshots

### Fenix 3
![Screenshot](https://github.com/eternal-flame-AD/git-notifications-ciq/blob/master/docs/img/git-notification-fenix3.png?raw=true)
### Forerunner 630
![Screenshot](https://github.com/eternal-flame-AD/git-notifications-ciq/blob/master/docs/img/git-notification-fr630.png?raw=true)
![Screenshot](https://github.com/eternal-flame-AD/git-notifications-ciq/blob/master/docs/img/git-notification-menu.png?raw=true)

## Usage


1. Install this Connect IQ(R) App on your watch.
1. Open the widget and complete OAuth to GitHub on your phone, or enter an personal access token in the application settings.
1. Enjoy!

## Features

- Notifications count

- Abbreviated notification type, source repo, and title

- Mark all as read

- Open notifications on your phone

## Known Limitations

- Due to the response body size limit by the Connect IQ SDK, only around 3-4 notifications could be received correctly. If the API response body size exceeded the limit, a "++" and an error message will appear indicating that there are too many notifications to be received from the GitHub API. My solution is to build an API gateway for the GitHub side which removed unnecessary fields from the API response and I think we would be able to receive at least 20 notifications then. This will be implemented in the future and the gateway feature will ONLY be used with the user's explicit consent in application settings. Also, the source code of the gateway would be publicized also and I would provide a way for users to build their own gateway on their own server and domains so that there would be no worries on the credential safety.

## TODO

- <s>Add OAuth support</s>

- Add If-Modified-After support

- (Maybe) Add GitLab support

## Disclaimer

- This Connect IQ(R) App is a personal project developed and open-sourced by [eternal-flame-AD](https://github.com/eternal-flame-AD). The application is neither affiliated to nor endorsed by GitHub, Inc. The application only sends requests to the already Github API publicized by GitHub, Inc. The use of the GitHub logo is only for the indication of GitHub notification count.

## Contributing

### Bug report and feature requests

Please report bugs and feature requests on [Github Issues](https://github.com/eternal-flame-AD/git-notifications-ciq/issues). Contacting through Connect IQ(R) Store is not guaranteed a response.

### Code contributions

Open up a PR on [GitHub](https://github.com/eternal-flame-AD/git-notifications-ciq/pulls) directly.

### Device support

I develop and test my application on my Forerunner 630 and my friend's Fenix 3. Other models might work as well, so if I didn't include your model into the build target, feel free to clone the repo and try sideloading the app onto your watch. If it works, just open a PR or issue to notify me and I will add your device to the build targets and issue a new version to the Connect IQ(R) Store. If there are some layout problems, try to fix it without breaking existing support and open a PR to have your layout update merged.

## LICENSE 

- This project is released and open-sourced on GitHub under the Apache License 2.0. You should receive a copy of the license together with the source code. If not, get it [here](https://github.com/eternal-flame-AD/git-notifications-ciq/blob/master/LICENSE).
