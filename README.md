# BiometryCam
🤖 Sistema de Reconhecimento Facial com Arduino + Computador
📋 Visão Geral do Sistema
Este projeto implementa um sistema de reconhecimento facial inteligente que combina o poder de processamento de um computador com a versatilidade de controle do Arduino.

text
┌─────────────────┐    Serial    ┌─────────────────┐
│   COMPUTADOR    │ ◄──────────► │    ARDUINO      │
│  (Processamento)│              │   (Controle)    │
└─────────────────┘              └─────────────────┘
         │                               │
         ▼                               ▼
    ┌─────────┐                     ┌─────────┐
    │ Câmera  │                     │ Atuadores│
    └─────────┘                     └─────────┘
🎯 Arquitetura do Sistema
Abordagem Híbrida
O Arduino atua como controlador que interage com um software de reconhecimento facial rodando em um computador externo.

✅ Vantagens Principais
🧠 Processamento Avançado: Utiliza o poder computacional do PC para algoritmos complexos

🎯 Alta Precisão: Reconhecimento facial mais preciso e confiável

🔧 Flexibilidade: Fácil atualização e modificação do software de visão

💡 Custo Efetivo: Não requer hardware especializado caro

🛠 Hardware Necessário
Componente	Descrição
🟦 Placa Arduino	Uno, Nano, Mega ou similar
📷 Câmera	Webcam USB conectada ao computador
💻 Computador	PC, Laptop ou Raspberry Pi
⚡ Componentes Adicionais	Servos, LEDs, travas elétricas
🖥 Software & Bibliotecas
Computador (Python)
python
# Bibliotecas principais
- OpenCV (visão computacional)
- pySerial (comunicação serial)
- NumPy (processamento numérico)
- face_recognition (opcional)
Arduino (C++)
cpp
// IDE Arduino para programação
#include <Servo.h>
#include <Wire.h>
🔄 Fluxo de Funcionamento
🎥 Captura de Imagem

Câmera conectada ao computador captura vídeo

Software Python processa os frames

🤖 Reconhecimento Facial

OpenCV detecta rostos na imagem

Algoritmo identifica pessoa específica (biometria)

📡 Comunicação Serial

Computador envia comando para Arduino via USB

Protocolo serial personalizado

⚡ Ação do Arduino

Arduino recebe comando

Aciona componentes (LEDs, servos, travas)

⚠️ Considerações Importantes
🚫 Limitações do Arduino
⚠️ Atenção: Placas Arduino básicas (Uno, Mega) não conseguem realizar reconhecimento facial sozinhas devido à limitação de processamento.

🔍 Diferenças Cruciais
Tipo	Descrição
Detecção Facial	Apenas localiza um rosto na imagem
Reconhecimento Facial	Identifica a pessoa específica (biometria)
📊 Comparação com Outras Biometrias
Tecnologia	Arduino	Processamento	Aplicação
Impressão Digital	Módulos dedicados (DY50, AS608)	Local	Identificação biométrica
Reconhecimento Facial	+ Computador	Externo	Identificação avançada
💡 Casos de Uso Ideais
🏠 Sistemas de segurança residencial

🏢 Controle de acesso corporativo

🎮 Projetos de automação e IoT

🔬 Prototipagem rápida de sistemas biométricos

