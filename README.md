# 🎯 Análise Exploratória da Mega-Sena (1996–2026)

"Tecnologias Utilizadas”:

Para reproduzir o projeto, instale as dependências descritas em requirements.txt.

Este projeto reúne uma análise completa dos sorteios da Mega-Sena desde 1996 até 2026, utilizando Python, Jupyter Notebook e visualizações estatísticas.  
O objetivo principal é explorar padrões históricos, distribuições e comportamentos dos números sorteados.

---

## 📌 Objetivos do Projeto

- Explorar o comportamento das dezenas ao longo dos anos  
- Avaliar distribuições estatísticas (como soma das dezenas)  
- Identificar padrões de paridade, faixas de valores e combinações  
- Criar visualizações claras e intuitivas  
- Realizar testes de normalidade  
- Preparar os dados para futura análise no Power BI  

---

## 🧠 Perguntas de Análise

- Quais dezenas são mais sorteadas?  
- A soma das dezenas segue uma distribuição próxima do normal?  
- Qual a frequência de combinações pares/ímpares?  
- Como os sorteios se distribuem ao longo dos meses e anos?  
- Existem dezenas com períodos longos sem serem sorteadas?  

---

## 🛠 Tecnologias Utilizadas

- **Python 3.10+**  
- **Jupyter Notebook**  
- **Pandas**  
- **NumPy**  
- **Seaborn**  
- **Matplotlib**  
- **SciPy** (testes de normalidade)

---

## 📂 Estrutura do Projeto


📁 mega-sena-analise
├── 📁 data
│ └── Mega_Sena.xlsx
├── 📁 notebooks
│ └── mega_sena_analise.ipynb
├── requirements.txt
└── README.md


---

## 🔍 Etapas da Análise

### 1. Carregamento dos Dados  
Leitura do dataset oficial da Caixa contendo concursos, dezenas e dados complementares (ganhadores, rateios, acumulados etc).

### 2. Limpeza e Tratamento  
- Conversão de datas  
- Criação de colunas: ano, mês  
- Verificações de duplicidade e consistência  

### 3. Engenharia de Atributos  
Criamos métricas importantes como:  
- soma_dezenas  
- media_dezenas  
- qtd_pares  
- qtd_impares  
- range das dezenas  
- década das bolas  
- sequência ordenada  
- distribuição das dezenas em lista única  

### 4. EDA — Análise Exploratória  
Inclui:  
- Frequência das dezenas  
- Histograma da soma  
- Histograma do range  
- Heatmap mensal/anual  
- Boxplots  
- Séries temporais  
- Testes estatísticos de normalidade (Shapiro-Wilk e KS)

### 5. Visualizações  
Todos os gráficos foram construídos com Matplotlib e Seaborn, organizados no notebook.

---

## 📊 Principais Insights Encontrados

- A soma das dezenas apresenta comportamento próximo de uma distribuição normal.  
- A combinação mais comum é **3 pares e 3 ímpares**.  
- O range dos sorteios geralmente fica na faixa de **40 a 50**.  
- Algumas dezenas aparecem com destaque ao longo das décadas.  
- Os meses com mais sorteios são **dezembro e outubro** (devido à Mega da Virada e calendário da Caixa).  

---

## 🧪 Testes Estatísticos

Realizamos:

- **Shapiro-Wilk** para amostras menores  
- **Kolmogorov-Smirnov** para comparação da distribuição teórica  

Ambos aplicados à distribuição da soma das dezenas.

---

## 📈 Próximo Passo: Power BI

Utilizaremos o dataset tratado e enriquecido para:

- Criar dashboards interativos  
- Explorar dezenas mais recorrentes  
- Analisar curvas de distribuição  
- Visualizar evolução de sorteios e acumulados  
- Apresentar combinações clássicas

---

## 🚀 Como Executar o Projeto

1. Clone o repositório:

git clone https://github.com/seuusuario/mega-sena-analise.git

2. Crie o ambiente virtual:

python -m venv venv


3. Ative o ambiente:

Windows:

venv\Scripts\activate


Linux/Mac:

source venv/bin/activate


4. Instale as dependências:

pip install -r requirements.txt


5. Abra o Jupyter Notebook:  

jupyter notebook


---

## 📬 Contato

📧 Email: luis.antonio1979@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/luisantonioalvesg  
🐍 Projetos em dados, ETL, Python e BI

---

## 📜 Licença
Este projeto é distribuído sob a licença MIT.

---

🟢 *Este repositório será atualizado regularmente conforme novos recursos forem adicionados, incluindo Power BI e relatórios finais.*
