# ❄️ AirLink Firmware (ESP8266 IoT)

[![C++](https://img.shields.io/badge/Language-C%2B%2B%20%2F%20Arduino-00979D?style=for-the-badge&logo=arduino)](https://www.arduino.cc/)
[![ESP8266](https://img.shields.io/badge/Hardware-ESP8266-E7352C?style=for-the-badge&logo=espressif)](https://www.espressif.com/)
[![Protocol](https://img.shields.io/badge/IR-Infrared%20Remote-darkgreen?style=for-the-badge)](#)

Firmware embarcado em **C++ / Arduino** para o microcontrolador **ESP8266** para acionamento remoto de aparelhos de ar-condicionado via emissor infravermelho (IR).

---

## 📌 Sobre o Projeto

O **AirLink Firmware** conecta o microcontrolador ESP8266 à rede Wi-Fi e atua como uma ponte entre requisições HTTP seguras (HTTPS) da API AirLink (`airlink-api`) e os comandos infravermelhos recebidos pelo aparelho de ar-condicionado, permitindo ligar, desligar, alterar temperatura e alternar modos de operação à distância.

## 🚀 Funcionalidades

- 📶 **Wi-Fi Seguro:** Conexão a redes sem fio com suporte a cliente HTTPS (`WiFiClientSecure`).
- 📡 **Emissão de Sinais IR:** Envio de pacotes infravermelhos codificados via biblioteca `IRremoteESP8266`.
- 🌡️ **Comandos Suportados:** Power On/Off, ajuste de temperatura, velocidade de ventilação e modo (Cool/Dry/Fan).

## 🛠️ Hardware Necessário

- **Placa ESP8266** (NodeMCU ou Wemos D1 Mini)
- **LED Emissor Infravermelho (940nm)** conectado ao pino digital (D1 / GPIO 5)
- Transistor NPN (ex: 2N2222) e resistores para amplificação do sinal IR

## ⚙️ Como Gravar no Microcontrolador

1. Abra o arquivo `Projeto_Airlink_Micro.ino` na **Arduino IDE**.
2. Instale o pacote de placas ESP8266 e a biblioteca **`IRremoteESP8266`**.
3. Configure o SSID e senha da sua rede Wi-Fi nas constantes do código.
4. Selecione a porta COM correspondente e clique em **Carregar (Upload)**.

---

## 👤 Autor

Desenvolvido por **[Iury Almeida](https://github.com/IuryAlmeidaDev)**.
