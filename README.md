# 🌱 Plantinha Inteligente IoT — Monitoramento com Animações + MQTT
<p align="center"> <img src="https://img.shields.io/badge/Status-Ativo-green?style=for-the-badge"/> <img src="https://img.shields.io/badge/Plataforma-ESP32-blue?style=for-the-badge"/> <img src="https://img.shields.io/badge/Protocolo-MQTT-purple?style=for-the-badge"/> <img src="https://img.shields.io/badge/Simulação-Wokwi-orange?style=for-the-badge"/> </p>

## 👤 INTEGRANTE | RM | GITHUB

* [Gabriela Abdelnor Tavares](https://github.com/GabihAbdTavares) - 562291
* [Maria Eduarda Sousa Acyole de Oliveira](https://github.com/MariaEduardaAcyole) – 566337
* [Matheus Goes](https://github.com/Goes1404) - 566407


## 🌱 1. Identificação do Problema

Com a rotina acelerada do futuro do trabalho, ambientes corporativos precisam oferecer bem-estar e equilíbrio emocional. Elementos naturais — como plantas — ajudam a reduzir estresse e melhorar a produtividade.

Mas muitas vezes:
- ❌ As plantas são esquecidas
- ❌ Falta monitoramento constante
- ❌ Não existe engajamento com o cuidado

➡️ Assim nasceu a Plantinha Inteligente IoT: uma solução divertida e útil para incentivar o cuidado com o si mesmo.

## ✨ 2. Solução Proposta
A solução combina:

- ✔ ESP32
- ✔ Sensores de Umidade e Luz
- ✔ LCD 16x2 com carinha animada
- ✔ Comunicação MQTT em tempo real
- ✔ Simulação no Wokwi

A plantinha reage às condições com animações (feliz, neutra, triste), e os dados são enviados para um broker MQTT, permitindo monitoramento remoto.


## 3. ☁️ Comunicação MQTT — Explicação Técnica

Usamos o broker público:

``` broker.hivemq.com```
```Porta: 1883```

## 4. 📡 Tópicos utilizados:
| Tópico MQTT | Descrição | Payload |
|-------------|-----------|---------|
| `plantinha/umidade` | Envia a umidade do solo | int |
| `plantinha/luz` | Envia a luminosidade | int |
| `plantinha/status` | Estado emocional (Feliz / Atenção / Triste) | string |

## 🔌 5. Componentes

| Componente | Função |
|-----------|--------|
| **ESP32** | Processamento + Internet |
| **Sensor de Umidade (simulado com potenciômetro)** | Mede a umidade do solo |
| **LDR** | Mede a luminosidade |
| **LCD 16x2 I2C** | Exibe as expressões da planta |
| **MQTT (HiveMQ)** | Envia dados em tempo real |

---

## 🛠️ 6. Link da Simulação no Wokwi

👉 **Simulação Pública:**  
https://wokwi.com/projects/SEU-LINK-AQUI

---

## 🎥 7. Vídeo Explicativo

👉 **Vídeo completo:**  
https://youtube.com/SEU-LINK-AQUI

---

## 🧪 8. Demonstração e Funcionamento

A lógica emocional da planta funciona assim:

| Emoção | Condição |
|--------|----------|
| 😀 **Feliz** | Umidade alta e boa luz |
| 😐 **Atenção** | Níveis medianos |
| 😢 **Triste** | Baixa umidade ou pouca luz |

Além disso, a plantinha **pisca os olhos ocasionalmente**, criando um comportamento mais realista ✨

---

## 💻 9. Código-Fonte 

O código completo está disponível em:  
`/src/plantinha.ino`

## 🧩 11. Como Reproduzir
- ✔ 1. No Wokwi

Use o WiFi padrão:

```ssid = "Wokwi-GUEST";```
```password = "";```

- ✔ 2. No App MyMQTT
Host/Broker: broker.hivemq.com
Porta: 1883

Assine os tópicos:

- plantinha/umidade
- plantinha/luz
- plantinha/status

## 🌍 12. Impacto no Futuro do Trabalho
A solução contribui para:
- ✔ Ambientes mais saudáveis
- ✔ Engajamento entre colaboradores
- ✔ Estímulo ao cuidado coletivo
- ✔ Aplicação real de IoT no ambiente corporativo
- ✔ Proposta divertida, leve e humanizada

Ideal para empresas que desejam integrar tecnologia + bem-estar no dia a dia.

## 🎯 13. Conclusão
A Plantinha Inteligente IoT une tecnologia, bem-estar e criatividade.
É uma solução prática, replicável e mostra, na prática, como IoT pode transformar ambientes de trabalho em espaços mais vivos, leves e eficientes.


