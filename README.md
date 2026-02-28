# Projeto 6 - Clusterização de Municípios Brasileiros

Clusterização de municípios brasileiros utilizando indicadores de desmatamento (PRODES), uso do solo (MapBiomas) e classificação por biomas (IBGE).

---

## 📌 Objetivo

Identificar padrões estruturais de desmatamento municipal no Brasil por meio de técnicas de aprendizado não supervisionado.

---

## 📊 Bases de Dados

- PRODES (INPE) – Série histórica até 2025
- MapBiomas – Cobertura do solo até 2024
- IBGE – Classificação municipal por bioma

⚠ Os arquivos de dados não estão incluídos neste repositório devido ao tamanho (~209MB).

Para reproduzir a análise, baixe os dados no link abaixo e coloque-os em uma pasta local:

📂 Google Drive:
https://drive.google.com/drive/folders/1Co3-RYMXHWkBeOx1aKnkZIj6W0SCywIE?usp=sharing

---

## 🛠 Metodologia

1. Pré-processamento e engenharia de atributos
2. Análise Exploratória (EDA)
3. Redução de dimensionalidade (PCA)
4. Clusterização:
   - K-Means
   - Hierárquico (Ward)
   - DBSCAN (exploratório)
5. Validação por métricas internas:
   - Silhouette
   - SSE (cotovelo)
   - ARI / NMI (estabilidade)

---

## 📈 Principais Resultados

- Melhor número de clusters: k = 2
- Silhouette K-Means ≈ 0.79
- Silhouette Ward ≈ 0.80
- Alta estabilidade (ARI > 0.98)
- Dois regimes territoriais distintos identificados

---

## ▶ Como Executar

### Opção 1 – Google Colab
Abrir o notebook `.ipynb` no Google Colab e fazer upload manual dos arquivos de dados.

### Opção 2 – Jupyter Notebook local

Instalar dependências e executar:
pip install -r requirements.txt
jupyter notebook

Abrir o arquivo:
Projeto6_Clusters.ipynb


---

## 📄 Relatório

O relatório técnico completo encontra-se na pasta `RELATORIO/`.

---

Autores:
Gustavo Antunes  
Millena Lins

UFU – FACOM – Ciência de Dados II
