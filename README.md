# Dataset para o TCC: "Gêmeo Digital Multi-Camada"

Este repositório contém o dataset utilizado no trabalho de conclusão de curso intitulado **"Gêmeo Digital Multi-Camada"**.

## Componentes do Dataset

O dataset é composto por dois arquivos: 'dataset_dados.txt' e 'dataset_ações.txt'. O primeiro contém dados sintéticos que são utilizados para alimentar o gêmeo digital. Este arquivo inclui medições de frequências cardíacas (BPM) e níveis de bateria dos dispositivos. Enquanto o segundo registra as respostas geradas pelo gêmeo digital com base nas entradas fornecidas pelo dataset_dados.txt. O gêmeo digital analisa os dados recebidos e somente retorna uma ação quando detecta uma situação de risco para o sistema.

1. **dataset_dados.txt**:
   - **Descrição**: Este arquivo contém medições de frequências cardíacas (BPM) e níveis de bateria de dispositivos (relógio e celular) em vários momentos. Esses dados são utilizados para alimentar o gêmeo digital e simular o comportamento dos dispositivos.
   - **Formato**: JSON
   - **Exemplo de entrada**:
     ```json
     {"bpm": 70.0, "watchBattery": 100.0, "cellphoneBattery": 100.0, "datetime": "2024-07-18 19:30:56"}
     {"bpm": 69.7, "watchBattery": 100.0, "cellphoneBattery": 100.0, "datetime": "2024-07-18 19:31:26"}
     ```

2. **dataset_ações.txt**:
   - **Descrição**: Este arquivo contém as respostas geradas pelo gêmeo digital para as diferentes entradas do primeiro dataset. O dado "timeDiff" foi utilizado para cálculos de delay, não estando presentes nas respostas originais do gêmeo.
   - **Formato**: JSON
   - **Exemplo de entrada**:
     ```json
     {"UPDATE_CELLPHONE_FREQUENCY": 5, "datetime": "2024-07-18 22:22:26", "timeDiff": "0:0:3:17"}
     {"UPDATE_CELLPHONE_FREQUENCY": 5, "datetime": "2024-07-18 22:24:56", "timeDiff": "0:0:1:339"}
     ```

## Objetivos do Dataset

- **Avaliar o Modelo de Gêmeo Digital**: O dataset é crucial para testar a eficácia do modelo do gêmeo digital.
- **Visualizar e Interpretar Dados**: O dataset facilita a criação de gráficos e análises para compreender como as variações nos dados influenciam as respostas do gêmeo digital.


# Visualização dos dados:
![GRÁFICO](https://github.com/user-attachments/assets/bdf2480b-46a7-459f-9d56-d6719f83e2cf)
