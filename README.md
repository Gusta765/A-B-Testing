# 🧪 A/B Testing — Metodologia Científica para Testar Hipóteses

O A/B Testing é uma técnica estatística usada para comparar duas ou mais versões de uma variável (como uma interface, funcionalidade ou algoritmo) e verificar, com rigor científico, qual delas gera melhores resultados. 

Neste projeto, simulamos um experimento em que diferentes algoritmos e elementos visuais (como um botão vermelho de "Reservar Agora") foram testados com o objetivo de aumentar a taxa de reservas em um site de restaurantes.

Rodamos a análise com Python, aplicando testes estatísticos, métricas de conversão e segmentações por tipo de restaurante.

# Legenda da base de dados
![image](https://github.com/user-attachments/assets/ee9db8f4-b8e5-4aef-b8a4-e4c2c8f07ca4)

## 🧪 Objetivo

Comparar estatisticamente o desempenho de três grupos:
- **Grupo Controle** (sem algoritmo)
- **Algoritmo Atual**
- **Novo Algoritmo**

---

## 🔍 Metodologia

- Leitura de dados via **Pandas** a partir de planilha Excel.
- Cálculo de **taxas de conversão** e **taxas de clique**.
- Aplicação de **Testes T de Student** (via `scipy.stats`) para avaliar significância estatística entre os grupos.
- Análise segmentada por tipo de restaurante (franquia vs. independente).
- Visualizações com **Seaborn** e **Matplotlib** (não exibidas aqui, mas prontas para uso).

---

## 📈 Resultados

### ➕ Taxa Média de Conversão

| Grupo              | Conversão (%) |
|--------------------|---------------|
| Controle           | 17.50%        |
| Algoritmo Atual    | 15.06% ⬇️     |
| Novo Algoritmo     | 18.73% ⬆️     |

- **Algoritmo Atual** teve uma **queda de 13.97%** na conversão.
- **Novo Algoritmo** apresentou um **ganho de 7.03%**.

### 📊 P-valores (Significância Estatística)

- Controle vs. Algoritmo Atual: `p < 0.0001`
- Controle vs. Novo Algoritmo: `p < 0.0001`

> Resultado estatisticamente significativo com 99% de confiança.

---

## 🏪 Análise por Tipo de Restaurante

### Restaurantes **Independentes**

| Grupo              | Conversão (%) |
|--------------------|---------------|
| Controle           | 20.24%        |
| Algoritmo Atual    | 16.94% ⬇️     |
| Novo Algoritmo     | 21.93% ⬆️     |

- **+8.35%** de ganho com o novo algoritmo.

### Restaurantes **Franquia**

| Grupo              | Conversão (%) |
|--------------------|---------------|
| Controle           | 13.39%        |
| Algoritmo Atual    | 12.24% ⬇️     |
| Novo Algoritmo     | 13.90% ⬆️     |

- **+3.81%** de ganho com o novo algoritmo.

---

## ✅ Recomendações

- **Descontinuar imediatamente o Algoritmo Atual** — apresenta perdas consistentes em todos os segmentos.
- **Implementar o Novo Algoritmo** — ganho estatisticamente significativo em ambos os tipos de restaurante.
- **Para restaurantes independentes**: prioridade na migração e materiais de treinamento específicos.
- **Para franquias**: implementar com monitoramento e possíveis ajustes finos.

---

## 🛠️ Ferramentas Utilizadas

- `Python` · `Pandas` · `Scipy` · `NumPy`
- `Seaborn` · `Matplotlib`
- **Testes A/B** · **Extração de insights de negócio**

---

## 📫 Contato

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gustavo-barbosa-868976236/)
[![Email](https://img.shields.io/badge/Email-gustavobarbosa7744@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gustavobarbosa7744@gmail.com)

---

> Este projeto demonstra minha capacidade de realizar testes estatísticos rigorosos, gerar insights acionáveis e tomar decisões baseadas em dados — habilidades essenciais para atuar como **Analista ou Cientista de Dados** em empresas com maturidade analítica.
