# pigpio

Wraps the C control lib [pigpio](https://github.com/joan2937/pigpio) in a Home Assistant addon to allow an easy installation.

![Addon Stage][stage-badge]
![Supports aarch64 Architecture][aarch64-badge]
![Supports amd64 Architecture][amd64-badge]
![Supports armhf Architecture][armhf-badge]
![Supports armv7 Architecture][armv7-badge]
![Supports i386 Architecture][i386-badge]

[![Add repository on my Home Assistant][repository-badge]][repository-url]
[![Install on my Home Assistant][install-badge]][install-url]
[![Donate][donation-badge]][donation-url]

## Usage

This addon runs the pigpio deamon which listens on http commands and control the GPIO on a Raspberry Pi accordingly (currently only up to PI 4).
Running this and using the [remote_rpi_pgio integration](https://www.home-assistant.io/integrations/remote_rpi_gpio/) in your Home Assistant configuration pointing to `localhost` will connect both worlds.

For additional options for the deamon use the optional addon setting `additional_options`.
The options`-g -f` will be always set!

## Security

It accesses `/dev/mem` on the host and also has full access to the raw io data.

[stage-badge]: https://img.shields.io/badge/Addon%20stage-stable-green.svg
[aarch64-badge]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-badge]: https://img.shields.io/badge/amd64-no-red.svg
[armhf-badge]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-badge]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-badge]: https://img.shields.io/badge/i386-no-red.svg

[repository-badge]: https://img.shields.io/badge/Add-repository-41BDF5?logo=home-assistant&style=for-the-badge
[repository-url]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A//github.com/Poeschl-HomeAssistant-Addons/repository

[install-badge]: https://img.shields.io/badge/Install%20on-Home%20Assistant-41BDF5?logo=home-assistant&style=for-the-badge
[install-url]: https://my.home-assistant.io/redirect/supervisor_addon?addon=68413af6_pigpio

[donation-badge]: https://img.shields.io/badge/Buy%20me%20a%20coffee-%23d32f2f?logo=buy-me-a-coffee&style=for-the-badge&logoColor=white
[donation-url]: https://www.buymeacoffee.com/Poeschl

