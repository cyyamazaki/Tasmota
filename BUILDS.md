## Recursos e sensores disponíveis

Este fork compila um único build (`tasmota-1M-essential`, ESP8266 1M). A tabela original do Tasmota, que comparava recursos entre as variantes `lite`/`tasmota`/`knx`/`sensors`/`ir`/`display`, não se aplica — essas variantes foram removidas deste repositório (veja o [README.md](README.md)).

### O que está habilitado em `tasmota-1M-essential`

| Recurso | Estado |
| --- | --- |
| Relé / Switch / Botões | Habilitado |
| Timers | Habilitado |
| Rules (regras) | Habilitado |
| MQTT / Web UI / OTA | Habilitado |
| Tasmota Discovery | Habilitado |
| DHT11 / DHT22 / AM2301 | Habilitado |
| DS18x20 | Habilitado |
| HTU21 / SI7021 (I2C) | Habilitado |
| BMP/BME280 (I2C) | Habilitado |
| Dimmer / Light (WS2812, MY92X1, SM16716/2135/2335, etc.) | Removido |
| Monitoramento de energia | Removido |
| Display | Removido |
| KNX / DALI | Removido |
| Zigbee | Removido |
| Berry (scripting) | Removido |
| IR remoto | Removido |
| ESP32 (toda a plataforma) | Removido |
| Demais sensores I2C, RF, LoRa, GPS, CO2/particulados, RFID, etc. | Removido |

A lista completa de macros `USE_*` habilitadas/desabilitadas está em `tasmota/include/tasmota_configurations.h`, bloco `FIRMWARE_ESSENTIAL`.

Para a matriz completa de builds oficiais do Tasmota, veja o projeto original: https://github.com/arendst/Tasmota/blob/development/BUILDS.md
