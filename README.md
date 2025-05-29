# AgriSmart
# AgriSmart – Sistema Inteligente de Irrigação com MQTT

O AgriSmart é um sistema de irrigação inteligente baseado em IoT, desenvolvido com ESP32, sensor de umidade do solo, módulo relé e uma bomba d’água. Seu objetivo é automatizar o controle da irrigação, promovendo o uso racional da água com monitoramento e acionamento remoto via protocolo MQTT.

## 🌱 Motivação

Este projeto foi escolhido por estar diretamente relacionado à minha vivência pessoal e por contribuir com o **Objetivo de Desenvolvimento Sustentável 9 (ODS 9)** da ONU, que incentiva a inovação e o uso de tecnologia para infraestrutura sustentável. A proposta visa democratizar o acesso à automação agrícola, especialmente para pequenos produtores.

## ⚙️ Funcionalidades

- Leitura contínua da umidade do solo
- Acionamento automático da bomba d’água quando o solo estiver seco
- Publicação dos dados de umidade em um tópico MQTT
- Recebimento de comandos remotos (ligar/desligar) via MQTT

## 🧪 Tecnologias Utilizadas

- **Microcontrolador:** ESP32
- **Sensor:** FC-28 (umidade do solo)
- **Atuador:** Módulo relé 5V e bomba d’água submersível
- **Comunicação:** Protocolo MQTT sobre TCP/IP
- **Broker MQTT:** HiveMQ (broker público)
- **Simulação:** Wokwi

## 🌐 Tópicos MQTT

- `agrismart/umidade` – Publica o valor lido do sensor
- `agrismart/comando` – Recebe comandos `"ligar"` ou `"desligar"`


## 📦 Estrutura do Projeto

- `sketch.ino` – Código principal do ESP32
- `diagram.json` – Diagrama da simulação no Wokwi
- `project.json` – Arquivo de configuração do projeto
- `docs/` – Imagens e capturas do sistema em funcionamento
- `hardware/` – Lista de componentes utilizados
- `protocolo/` – Documentação da comunicação MQTT

## 📽️ Vídeo Demonstração

Apresentação completa do sistema, incluindo hardware, código e teste com protocolo MQTT:  
🔗 (https://youtu.be/kpqkQivZMP0)](https://www.youtube.com/watch?v=Uh2IeL__LEA)

---

