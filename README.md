# BiometryCam  
🤖 **Sistema de Reconhecimento Facial com Arduino + Computador**

---

## 📋 Visão Geral do Sistema
Este projeto implementa um sistema de reconhecimento facial inteligente que combina o poder de processamento de um computador com a versatilidade de controle do Arduino.

---

## 🎯 Arquitetura do Sistema

### **Abordagem Híbrida**
O Arduino atua como controlador que interage com um software de reconhecimento facial rodando em um computador externo.

### ✅ **Vantagens Principais**
- 🧠 **Processamento Avançado:** Usa o poder computacional do PC para algoritmos complexos  
- 🎯 **Alta Precisão:** Reconhecimento facial mais preciso e confiável  
- 🔧 **Flexibilidade:** Fácil atualização e modificação do software de visão  
- 💡 **Custo Efetivo:** Não requer hardware especializado caro  

---

## 🛠 Hardware Necessário

| Componente | Descrição |
|-----------|-----------|
| 🟦 **Placa Arduino** | Uno, Nano, Mega ou similar |
| 📷 **Câmera** | Webcam USB conectada ao computador |
| 💻 **Computador** | PC, Laptop ou Raspberry Pi |
| ⚡ **Componentes Adicionais** | Servos, LEDs, travas elétricas |

---

## 🖥 Software & Bibliotecas

### **Computador (Python)**

```python
# Bibliotecas principais
- OpenCV (visão computacional)
- pySerial (comunicação serial)
- NumPy (processamento numérico)
- face_recognition (opcional)
