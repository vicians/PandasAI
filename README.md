🚀 Resumo das Alterações

Este PR adiciona a resolução do exercício prático focado em análise de dados e machine learning exploratório. O objetivo central foi integrar um modelo de linguagem (LLM) diretamente a um DataFrame para automatizar previsões usando regressão linear.

## 🛠️ O que foi implementado?

* **Integração LLM + Dados:** Configuração do `PandasAI` utilizando a API do Google Gemini (`gemini-2.5-flash`).
* **Workaround de Configuração:** Injeção manual do modelo atualizado na classe base da biblioteca para contornar limitações de versão (Erro 404).
* **Tratamento de Dados (RegEx):** Criação de uma função de extração numérica baseada em expressões regulares para tratar as respostas em linguagem natural da IA.
* **Machine Learning:** Previsão de salários baseada em `idade` e `anos_experiencia` utilizando regressão linear.
* **Visualização de Dados:**
  * Mapa de calor (Heatmap) com `Seaborn` para análise de correlação entre variáveis.
  * Gráfico de dispersão 3D com `Matplotlib` contrastando os dados originais com as novas previsões.

## 💻 Tecnologias Utilizadas
- Python 3
- Pandas & PandasAI
- Matplotlib & Seaborn
- Scikit-Learn
- Google Generative AI (Gemini)