---
title: 
description: 
published: true
date: 2020-02-03T14:23:38.750Z
tags: 
---

# Apply for maintainership
If you want to become the official maintainer of Evolution X for your device, you will need to apply with a Google Form. You can find everything important related below.

## Official Support Guidelines & Rules

[Official Support Application](https://docs.google.com/forms/d/e/1FAIpQLSe6InJeF09OMKV1G6-o9z0qhSebqvPAv4xyAuF2Ex8g7zJhiA/viewform) | [XDA Thread Template](https://raw.githubusercontent.com/Evolution-X-Devices/official_devices/master/xda/xda_template.txt) | [Devices Repository](https://github.com/Evolution-X-Devices)

Before you submit a pull request to add your device to our list of official devices, you should know a few simple things:

### 1. To become a maintainer of Evolution X:

1.2 - Maintainers must have a way to test their builds. Either owning the device, or sending builds to a reliable/trusted person to test for you. Completely blind and/or untested builds are not permitted.

1.3 - Applicants that physically own the device, will have the preference on receiving maintainship.

1.4 - You MUST have knowledge of git.

1.5 - You MUST compile an unofficial build and make the device stable for daily usage prior to submitting an appplication.

1.6 - You MUST have your device sources publicly available for us take a look at.

1.7 - You mustn't be a placeholder of another maintainer that was removed. Applications considered of that nature will not be accepted.

1.8 - If the device already have the active maintainer, you are not allowed to build any unofficial builds unless the maintainer resigned or removed.

### 2. Maintainers code of conduct:

2.1 - Maintainers MUST import their trees to https://github.com/Evolution-X-Devices

2.2 - Maintainers MUST test EVERY update before uploading/Pushing OTA.

2.3 - Maintainers MUST keep the authorship of Git commits, even if it's their device tree, kernel or vendor source. Lots of git commit --amend and force-push are acceptable.

2.4 - Relationship fights can be done via pm through Telegram or XDA.

2.5 - Maintainers will need to add/execute 'export CUSTOM_BUILD_TYPE=OFFICIAL' in/against their build environment in order to compile as OFFICIAL with OTA Updater.

2.6 - ROM source must not be modified in any way when releasing builds as OFFICIAL. If caught doing so, maintainership will be revoked without warning.

### 3. JSON Parameters

##### devices.json
| Param | Description | Required |
|--|--|--|
| name | Device name | Yes |
| brand | Device manufacturer | Yes |
| codename | Device codename, eg: tissot | Yes |
| version_code | Version code, lowercase, eg: pie | Yes |
| version_name | Version name, will be shown on download portal, eg: pie | Yes |
| maintainer_name | Your name | Yes |
| maintainer_url | Your personal URL, eg: https://github.com/stallix or https://forum.xda-developers.com/member.php?u=4936496 | No  |4936496
| xda_thread | XDA thread URL, eg: https://forum.xda-developers.com/mi-a1/development/rom-pe-evolution-t3901369 | No |


##### device_codename.json
| Param | Description | Required |
|--|--|--|
| filename | Build file (.zip) name | Yes |
| filesize | Build file (.zip) size (in bytes) | Yes |
| filehash | Build file (.zip) md5 hash | Yes |
| datetime | Build file (.zip) time | Yes |
| id | Build file (.zip)  hash | Yes |
| maintainer | your name | Yes |
| news_url | https://t.me/EvolutionXOfficial | Yes |
| website_url | https://evolution-x.org | Yes |
| forum_url | XDA Thread | Yes |
| telegram_username | Your telegram username | Yes |