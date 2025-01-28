# Controle de Temperatura com Q-Learning 🌡️

Este projeto aplica **Inteligência Artificial (IA)**, utilizando o algoritmo **Q-Learning**, para controlar a temperatura de um ambiente simulado. Uma interface gráfica, desenvolvida com **Tkinter**, permite que os usuários acompanhem a regulação da temperatura em tempo real.

---

## 📋 Descrição do Projeto

O sistema foi projetado para ajustar a temperatura do ambiente dentro de um intervalo ideal (20°C a 23°C) usando **Q-Learning**. O agente aprende, com base em tentativa e erro, as melhores ações para alcançar e manter a temperatura desejada.

---

## 🚀 Funcionalidades

1. **Treinamento com Q-Learning**: 
   - O sistema aprende a controlar a temperatura treinando com 5000 episódios.
   - Cria uma tabela \( Q \) que relaciona estados (temperatura atual) com ações (ajustar temperatura).

2. **Controle Dinâmico da Temperatura**:
   - O agente regula a temperatura em tempo real.
   - Exibe o status (temperatura ideal ou fora do intervalo).
   - Mostra um histórico das ações tomadas.

3. **Interface Gráfica**:
   - Exibe a temperatura atual e o status do sistema.
   - Mostra as ações realizadas pelo agente.
   - Botões para iniciar o controle ou fechar a aplicação.

---

## ⚙️ Tecnologias Utilizadas

- **Python**: Linguagem principal para desenvolvimento.
- **Tkinter**: Interface gráfica para interação com o usuário.
- **NumPy**: Para cálculos matemáticos e manipulação de arrays.

---

## 🛠️ Como o Sistema Funciona

1. **Treinamento com Q-Learning**:
   - O algoritmo cria uma tabela \( Q \) para relacionar estados de temperatura (15°C a 30°C) com as ações possíveis:
     - **Aumentar** a temperatura (+1°C).
     - **Diminuir** a temperatura (-1°C).
     - **Manter** a temperatura.
   - O sistema recebe uma recompensa com base na proximidade da temperatura ao intervalo ideal:
     - **+10** para temperaturas dentro do intervalo (20°C a 23°C).
     - Penalidade negativa proporcional ao desvio para temperaturas fora do intervalo.

2. **Controle em Tempo Real**:
   - A temperatura inicial é gerada aleatoriamente.
   - O agente ajusta a temperatura com base na melhor ação registrada na tabela \( Q \).
   - Exibe as mudanças e o histórico das ações na interface gráfica.

---

## 📝 Observações

- Este projeto é uma simulação com fins educacionais.
- O ambiente de controle é totalmente virtual e não interage com dispositivos físicos.

---
