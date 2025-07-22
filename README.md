Análise Estatística: Salários de Profissionais de Dados
Este repositório contém uma análise estatística detalhada sobre os salários de profissionais da área de dados, utilizando um script em Python. O objetivo é explorar um conjunto de dados para extrair insights sobre a remuneração, considerando fatores como cargo, nível de experiência, tamanho da empresa e localização geográfica.

📄 Sobre o Conjunto de Dados
A análise é baseada no arquivo salario_profissionais_dados.csv. Este dataset agrega informações salariais anônimas e as colunas mais relevantes para este estudo são:

job_title: O cargo específico do profissional (ex: Data Scientist, Data Engineer, Data Analyst).

experience_level: O nível de senioridade do profissional (ex: Entry-level, Mid-level, Senior, Executive).

company_size: O porte da empresa empregadora (Pequeno, Médio ou Grande).

country: O país onde o profissional está localizado.

work_year: O ano em que o dado salarial foi registrado.

salary_in_usd: O salário anual bruto em dólares americanos (USD), utilizado como métrica principal para comparações.

years_of_experience: A quantidade de anos de experiência do profissional.

🛠️ Tecnologias e Bibliotecas
A análise foi desenvolvida inteiramente em Python, com o auxílio das seguintes bibliotecas essenciais para manipulação e visualização de dados:

Pandas: Utilizada para a importação, limpeza e manipulação estruturada dos dados.

Matplotlib: Biblioteca fundamental para a criação de gráficos e visualizações estáticas.

Seaborn: Construída sobre o Matplotlib, é usada para criar visualizações estatísticas mais elaboradas e esteticamente agradáveis.

Instalação de Dependências
Para executar o script localmente, certifique-se de ter as bibliotecas necessárias instaladas. Você pode instalá-las via pip:

pip install pandas matplotlib seaborn

🚀 Como Executar a Análise
O código foi estruturado de forma sequencial, como em um notebook (Jupyter ou Google Colab), para facilitar a exploração passo a passo.

Clone o repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git

Navegue até o diretório do projeto:

cd seu-repositorio

Garanta que o arquivo salario_profissionais_dados.csv esteja no mesmo diretório que o script.

Execute o script. Recomenda-se o uso de um ambiente que permita a execução célula por célula para uma melhor interpretação dos outputs e gráficos gerados.

🔎 Estrutura da Análise
O script está organizado em cinco seções lógicas:

1. Importação e Exploração Inicial da Base
Nesta etapa inicial, o dataset é carregado e uma verificação preliminar é realizada para entender sua estrutura e qualidade.

Carregamento dos Dados: O arquivo .csv é lido para um DataFrame do Pandas.

Inspeção Estrutural: Funções como .head(), .info() e .shape são usadas para visualizar as primeiras linhas, verificar os tipos de dados de cada coluna e obter as dimensões do DataFrame.

Verificação de Dados Ausentes: O comando .isnull().sum() é utilizado para confirmar que não há valores nulos no conjunto de dados, garantindo a integridade da análise.

2. Frequência e Distribuição das Categorias
Aqui, investigamos a distribuição das principais variáveis categóricas para entender o perfil dos dados.

Cargos (job_title): Identificação dos 10 cargos mais frequentes.

Nível de Experiência (experience_level): Análise da proporção de profissionais em cada nível de senioridade.

Tamanho da Empresa (company_size): Verificação da distribuição de profissionais entre empresas de pequeno, médio e grande porte.

3. Estatísticas Descritivas
Esta seção foca na análise quantitativa da variável salary_in_usd.

Medidas de Tendência Central: Cálculo da média e mediana para identificar o centro da distribuição salarial.

Medidas de Dispersão: Cálculo do desvio padrão, mínimo e máximo para compreender a variabilidade e a amplitude dos salários.

Visualizações:

Histograma: Um gráfico da distribuição dos salários é gerado para visualizar sua forma, concentração e a presença de outliers.

Boxplot por Experiência: Um boxplot compara a distribuição salarial entre os diferentes níveis de experiência, evidenciando como a remuneração progride com a carreira.

4. Comparações por País
Exploramos como a remuneração varia geograficamente.

Os dados são agrupados por country para calcular a média salarial.

É gerada uma lista com os 10 países que apresentam as maiores médias salariais, oferecendo um panorama do mercado global.

5. Correlações e Tendências
A seção final investiga a relação entre as variáveis numéricas para identificar tendências.

Matriz de Correlação: É calculada a correlação de Pearson entre salary_in_usd, work_year e years_of_experience.

Mapa de Calor (Heatmap): A matriz de correlação é visualizada através de um heatmap, que facilita a identificação da força e da direção das relações. O principal objetivo é responder se existe uma tendência de aumento salarial conforme os anos de experiência aumentam.

📈 Principais Insights (Exemplos)
A análise de frequência revela que "Data Engineer" e "Data Scientist" estão entre os cargos mais comuns no dataset.

A distribuição salarial mostra uma assimetria positiva, sugerindo que, embora a maioria dos salários se concentre em uma faixa, existem alguns salários extremamente altos que elevam a média.

O nível de experiência é um forte preditor do salário, com uma clara progressão remuneratória dos níveis de entrada para os níveis sênior e executivo.

A análise de correlação confirma uma relação positiva e relevante entre os anos de experiência e o salário, validando a hipótese de que a remuneração tende a crescer com a experiência.
