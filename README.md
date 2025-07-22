# Análise Estatística: Salários de Profissionais de Dados

Este repositório contém uma análise estatística detalhada sobre os salários de profissionais da área de dados, utilizando um script em Python. O objetivo é explorar um conjunto de dados para extrair insights sobre a remuneração, considerando fatores como cargo, nível de experiência, tamanho da empresa e localização geográfica.

---

## 📄 Sobre o Conjunto de Dados

A análise é baseada no arquivo `salario_profissionais_dados.csv`. Este dataset agrega informações salariais anônimas e as colunas mais relevantes para este estudo são:

- **job_title**: O cargo específico do profissional (ex: Data Scientist, Data Engineer, Data Analyst).
- **experience_level**: O nível de senioridade do profissional (ex: Entry-level, Mid-level, Senior, Executive).
- **company_size**: O porte da empresa empregadora (Pequeno, Médio ou Grande).
- **country**: O país onde o profissional está localizado.
- **work_year**: O ano em que o dado salarial foi registrado.
- **salary_in_usd**: O salário anual bruto em dólares americanos (USD), utilizado como métrica principal para comparações.
- **years_of_experience**: A quantidade de anos de experiência do profissional.

---

## 🛠️ Tecnologias e Bibliotecas

A análise foi desenvolvida inteiramente em Python, com o auxílio das seguintes bibliotecas essenciais para manipulação e visualização de dados:

- **Pandas**: Para importação, limpeza e manipulação estruturada dos dados.
- **Matplotlib**: Biblioteca fundamental para a criação de gráficos e visualizações estáticas.
- **Seaborn**: Construída sobre o Matplotlib, usada para criar visualizações estatísticas mais elaboradas e esteticamente agradáveis.

### Instalação de Dependências

Para executar o script localmente, certifique-se de ter as bibliotecas necessárias instaladas. Use o comando:

```bash
pip install pandas matplotlib seaborn
