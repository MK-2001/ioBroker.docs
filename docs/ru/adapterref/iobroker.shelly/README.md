---
BADGE-NPM version: https://img.shields.io/npm/v/iobroker.shelly?style=flat-square
BADGE-Downloads: https://img.shields.io/npm/dm/iobroker.shelly?label=npm%20downloads&style=flat-square
BADGE-node-lts: https://img.shields.io/node/v-lts/iobroker.shelly?style=flat-square
BADGE-Libraries.io dependency status for latest release: https://img.shields.io/librariesio/release/npm/iobroker.shelly?label=npm%20dependencies&style=flat-square
BADGE-GitHub: https://img.shields.io/github/license/iobroker-community-adapters/iobroker.shelly?style=flat-square
BADGE-GitHub repo size: https://img.shields.io/github/repo-size/iobroker-community-adapters/iobroker.shelly?logo=github&style=flat-square
BADGE-GitHub commit activity: https://img.shields.io/github/commit-activity/m/iobroker-community-adapters/iobroker.shelly?logo=github&style=flat-square
BADGE-GitHub last commit: https://img.shields.io/github/last-commit/iobroker-community-adapters/iobroker.shelly?logo=github&style=flat-square
BADGE-GitHub issues: https://img.shields.io/github/issues/iobroker-community-adapters/iobroker.shelly?logo=github&style=flat-square
BADGE-GitHub Workflow Status: https://img.shields.io/github/actions/workflow/status/iobroker-community-adapters/iobroker.shelly/test-and-release.yml?branch=master&logo=github&style=flat-square
BADGE-Beta: https://img.shields.io/npm/v/iobroker.shelly.svg?color=red&label=beta
BADGE-Stable: http://iobroker.live/badges/shelly-stable.svg
BADGE-Installed: http://iobroker.live/badges/shelly-installed.svg
chapters: {"pages":{"de/adapterref/iobroker.shelly/README.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/README.md"},"de/adapterref/iobroker.shelly/protocol-coap.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/protocol-coap.md"},"de/adapterref/iobroker.shelly/protocol-mqtt.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/protocol-mqtt.md"},"de/adapterref/iobroker.shelly/restricted-login.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/restricted-login.md"},"de/adapterref/iobroker.shelly/state-changes.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/state-changes.md"},"de/adapterref/iobroker.shelly/faq.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/faq.md"},"de/adapterref/iobroker.shelly/debug.md":{"title":{"de":"ioBroker.shelly"},"content":"de/adapterref/iobroker.shelly/debug.md"}}}
translatedFrom: de
translatedWarning: Если вы хотите отредактировать этот документ, удалите поле «translationFrom», в противном случае этот документ будет снова автоматически переведен
editLink: https://github.com/ioBroker/ioBroker.docs/edit/master/docs/ru/adapterref/iobroker.shelly/README.md
title: ioBroker.shelly
hash: Uz3Ry8D/plZQTN+bQwUultYzPjqhk5vWw1PXNE8Owxw=
---
![логотип](../../../de/admin/shelly.png)

# IoBroker.shelly
Это немецкая документация - [🇺🇸Немецкая версия](../en/README.md).

## Оглавление
- [Протокол MQTT](protocol-mqtt.md)
- [Протокол CoAP/CoIoT](protocol-coap.md)
- [Ограниченный вход](restricted-login.md)
- [Изменения состояния](state-changes.md)
- [Отладка](debug.md)
- [FAQ](faq.md)

## Требования
1. Node.js 18 (или новее)
2. js-контроллер 5.0.19 (или новее)
3. Адаптер администратора 6.0.0 (или новее)

## Поколения устройств
Дополнительную информацию см. в разделе *поддерживаемые устройства*.

- **Поколение 1**: устройства ESP8266, [CoAP/CoIoT](protocol-coap.md) или [MQTT](protocol-mqtt.md).
- **Поколение 2+**: устройства ESP32, [MQTT](protocol-mqtt.md)

## В целом
Адаптер может обмениваться данными с устройствами через MQTT (рекомендуется) или CoAP/CoIoT.

- Режим адаптера по умолчанию — MQTT (дополнительную информацию см. в [Документации](protocol-mqtt.md)).
- CoAP/CoIoT совместим только с устройствами Gen1!
- **Если необходимо интегрировать устройства Gen2, необходимо настроить MQTT!**

Вопросы? Сначала взгляните на [Часто задаваемые вопросы](faq.md)!

![iobroker_general](../../../de/adapterref/iobroker.shelly/img/iobroker_general.png)

## Changelog

<!--
  Placeholder for the next version (at the beginning of the line):
  ### **WORK IN PROGRESS**
-->
### 8.2.1 (2024-09-23)

* (@Matze2010) Added datapoint for cover target position
* (@klein0r) Fixed integration of Shelly 1 PM Gen 3

### 8.2.0 (2024-09-19)

* (@Scrounger) Added Shelly BLU Wall Switch 4 & Shelly BLU RC Button 4
* (@Paradoxa) Added Shelly Plus RGBW PM
* (simatec) Responsive Design added

### 8.1.1 (2024-08-27)

* (@klein0r) Fixed lint issues and Shelly Gen 3 import

### 8.1.0 (2024-08-25)

* (esusxunil) Added Shelly Pro EM 2x50A

### 8.0.0 (2024-08-25)

* (imperial929) Added Shelly 1 PM Gen3
* (imperial929) Added Shelly 1 Gen3
* (klein0r) Breaking change: Renamed input states (now digital/analog) of Shelly Plus Addon (Ext)
* (klein0r) Added Shelly Plus Uni
* (klein0r) Added Shelly H&T (Gen3)
* (klein0r) Improved structure of ble events (receivedBy) - see documentation for details
* (bluefox) Improved the color of icons in the admin interface

## License

The MIT License (MIT)

Copyright (c) 2018-2024 Thorsten Stueben <thorsten@stueben.de>,
                        Apollon77 <iobroker@fischer-ka.de> and
                        Matthias Kleine <info@haus-automatisierung.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.