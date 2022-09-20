## :dna: Alura Challenge Data Science - 2
Esse desafio consiste em desenvolver e aplicar  habilidades de Data Science, Data Analytics e Machine Learning.

Briefing:
A Alura Cash disponibilizou os dados contidos no banco de dados quanto às informações de clientes que solicitaram créditos.

O desafio terá 4 semanas divididos em: 
* :pushpin: **Semana 1** - Tratamento de dados: entendendo como tratar dados com SQL :heavy_check_mark:
* :pushpin: **Semana 2** - Aprendendo com os dados: criando um modelo de previsão de inadimplência  
* :pushpin: **Semana 3 e 4** - Analisando métricas: criando visualizações com o Power BI

## Semana 1
### :mag: Overview
[Mais detalhes do processo aqui]()
 <br>
* Entender quais informações o conjunto de dados possui :heavy_check_mark:
* Analisar quais os tipos de dados :heavy_check_mark:
* Verificar quais são as inconsistências nos dados :heavy_check_mark:
* Corrigir as inconsistências nos dados :heavy_check_mark:
* Unir as tabelas de dados de acordo com os IDs :heavy_check_mark:
* Traduzir as colunas :heavy_check_mark:
* Exportar a tabela de dados unidos como csv :heavy_check_mark: 

#### Dados que iremos trabalhar
* **Person_id:** Id do solicitante **_(Qualitativo Nominal)_**
* **loan_id:** ID da solicitação de empréstico de cada solicitante  **_(Qualitativo Nominal)_**
* **cb_id:** ID do histórico de cada solicitante **_(Qualitativo Nominal)_**
* **person_Age:** Idade da pessoa - em anos - que solicita empréstimo **_(Quantitativo Discreto)_**
* **person_income:** salário anual da pessoa solicitante **_(Quantitativo discreto)_**
* **person_home_ownership:** Situação da propriedade que a pessoa possui: Alugada, Própria, Hipotecada e Outros **_(Qualitativo Nominal)_**
* **person_emp_length:** Tempo - em  anos - que a pessoa trabalhou **_(Qualitativo Ordinal)_**
* **loan_intent:** Motivo do empréstimo: Pessoal (Personal), Educativo (Education), Médico (Medical), Empreendimento (Venture), Melhora do lar (Homeimprovement), Pagamento de débitos (Debtconsolidation) **_(Qualitativo Nominal)_**
* **loan_grade:** Pontuação de empréstimos, por nível variando de A a G**  _(Qualitativo Ordinal)_**
* **loan_amnt:** Valor total do empréstimo solicitado  **_(Quantitativo discreto)_**
* **loan_int_rate:** Taxa de Juros  **_(Quantitativo Contínuo)_**
* **loan_status:** Possibilidade de inadimplência  **_(Qualitativo Nominal)_**
* **loan_percent_income:** Renda Percentual entre o valor total do empréstimo e o salário anual. **_(Quantitativa Ordinal)_**
* **cb_person_default_on_file:** Indica se a pessoa já foi inadimplente: sim(Y,YES) e não (N, NO) **_(Qualitativo nominal)_**
* **cb_person_cred_hist_length:** Tempo - em anos - desde a primeira solicitação de crédito ou aquisição de um cartão de crédito _**(Qualitativo ordinal)**_

#### Inconsistências 
* Realizei o replace de pd.NA para np.nan para facilitar a limpeza posterior, depois de verificar quais filtros deverão ser aplicados para o modelo.
* Verifiquei por coluna os valores vazios:<br>
![image](https://user-images.githubusercontent.com/61653788/191142078-0d23030a-4b8f-4f58-9c86-54b41de9e45f.png)


### Dataset final salvo 
Realizei a renomeação de algumas colunas para facilitar o entendimento durante a manipulação desses dados. 
![image](https://user-images.githubusercontent.com/61653788/191141756-c8145da6-c6ee-4ed9-a0a6-7d8c8b298bd4.png)
