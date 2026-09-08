# Local Apex Controller integration for [Home Assistant](https://www.home-assistant.io/)

This is a Home Assistant custom integration for the [Neptune Apex](https://www.neptunesystems.com/) line of aquarium controllers. It exposes supported controller inputs and outputs as Home Assistant sensors and switches.

## Project home and attribution

This repository, [cocojakes/apex-ha](https://github.com/cocojakes/apex-ha), is the maintained project home and the place to report issues or contribute changes.

It is based on the original [itchannel/apex-ha](https://github.com/itchannel/apex-ha) project. Full credit for the original integration, its architecture, and the foundation of this codebase goes to its original authors and contributors. This fork continues under the same GPL-3.0 license; see [LICENSE.md](LICENSE.md).

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/itchannel)

## Install

Use HACS and add this repository, `https://github.com/cocojakes/apex-ha`, as a custom integration repository. Once the integration is installed, go to **Settings → Devices & services → Integrations** and add **Apex**. You will need:

- Username (Apex Controller Username)
- Password (Apex Controller Password)
- Apex Controller IP Address

## Older versions (Apex Jnr, Apex Classic)

Older versions of the Apex controller don't support the rest API , however basic support has been added by @dkramarc which allows controlling switches and reading values using basic auth and the legacy API.

## Options

You can set the update interval that the integration polls the controller (in seconds), plus temperature (°C/°F) and length (in/cm) display units independently. Be aware you will need to reload the integration once updating options for this to take affect.

This is a community-built integration. It is not supported by or affiliated with Neptune Systems.

## Release history

### 2.0.0

The first release from the maintained `cocojakes/apex-ha` fork. It establishes this repository as the project home while preserving credit to the original project, and includes COR-20, LLS, MXM, `tdata`, and current Home Assistant options-flow support.
