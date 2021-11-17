# The Kraken Project
## Official devices application

Devices repository: [AOSPK-Devices](https://github.com/AOSPK-Devices)

Before you apply to add your device into our list of official devices, you should know a few things:

### 1. How to apply?

You must fulfill the following requirements before applying:

- [Maintainers requirements](https://github.com/AOSPK/official_devices/blob/master/docs/maintainers_requirements.md)

- [Device requirements](https://github.com/AOSPK/official_devices/blob/master/docs/device_requirements.md)

- [Maintainers' code of conduct](https://github.com/AOSPK/official_devices/blob/master/docs/maintainers_code_of_conduct.md)

You must be aware that just fulfilling these requirements doesn't necessarily mean that you're going to be accepted. We will also consider some other points if necessary, like experience or how your behavior is towards other people (users or otherwise), and even with some technical stuff.

If you agree with everything, and want to apply [**fill this form**](https://github.com/AOSPK/official_devices/issues/new/choose)

### 2. OTA and Hosting

Our OTA system is automatic, you should not worry about updating some script. The builds are hosted on our own server. You must build the official releases on our CI, no builds outside of it can be released as official. After the build is tested, you may release it.

### 3. JSON params

##### devices.json
| Param | Description | Required |
|--|--|--|
| brand | Device manufacturer | Yes |
| name | Device name | Yes |
| codename | Device codename, eg: beryllium | Yes |
| xda_thread | Direct url of your XDA profile (eg: https://forum.xda-developers.com/t/rom-11-0-beryllium-aospk-the-kraken-project-2020-12-16.4202055/) | No |
| supported_versions | Version name (pie, ten, eleven) | Yes |
| supported_types | Version code (gapps or vanilla) | Yes |
| deprecated | Set to true if the device is no longer maintained (false by default) | No |
| repositories | Array containing needed repositories by your device | Yes |

##### team/maintainers.json
| Param | Description | Required |
|--|--|--|
| name | Your name (or nickname) | Yes |
| country | ISO-3166 Alpha 2 code of your country (2 digits, you can get from https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) | Yes |
| github_username | Your GitHub username (eg: https://github.com/mamutal91/) | Yes |
| telegram_username | Direct url of your telegram profile | No |
| xda_url | Direct url of your XDA profile (eg: https://forum.xda-developers.com/m/mamutal91.8414586/) | No |
| devices | Array with the device and the respective version that you maintain | Yes |
| ci_username | Alphanumeric username, to be used in our CI | Yes |

### 4. Device Banner

Our banners are automatically generated, and you can use them to publish in communities on your device. [Download the image here!](https://github.com/AOSPK/official_devices/tree/master/images/banners)
