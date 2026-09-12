## Firmware deste fork

Este repositório é um fork reduzido do Tasmota (veja o [README.md](README.md)) que compila **apenas um firmware**:

| Ambiente PlatformIO | Placa alvo | Escopo |
| --- | --- | --- |
| `tasmota-1M-essential` | ESP8266 1M (`esp8266_1M`) | Relé/switch, botões, timers, regras, MQTT/Web/OTA + sensores DHT, DS18x20, HTU21/SI7021, BMP/BME280 |

Para compilar:

```
pio run -e tasmota-1M-essential
```

O binário resultante fica em `build_output/firmware/`.

Não há outros ambientes disponíveis (a matriz original de builds do Tasmota — `tasmota`, `tasmota-lite`, `tasmota-minimal`, `tasmota-sensors`, `tasmota-knx`, `tasmota-display`, `tasmota-ir`, `tasmota-zbbridge`, `tasmota-zigbee`, os builds ESP32 e as ~30 traduções — foi removida deste fork por não se aplicar ao uso pretendido). Para essas variantes, use o projeto original: https://github.com/arendst/Tasmota

### Personalização em tempo de compilação

Para mudar configurações sem alterar `my_user_config.h`, copie `tasmota/user_config_override_sample.h` para `tasmota/user_config_override.h` (ignorado pelo git) e ajuste ali.
