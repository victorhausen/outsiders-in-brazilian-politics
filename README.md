# Outsiders in Brazillian Deputies Chamber

In Brazil data on political candidatures are provided by the Supreme Electoral Court.
It's messy and scattered over more than 300 .txt and .csv files.

In this project is an attempt to properly wrangle and unify everything in a single MySQL relational database.

The project architecture is base arount 3 main folders:
* The code folder, where you can find the jupyter notebooks.
* The data folder where all data is stored. The whole dataset has not been uploaded here because its massive,
but you an generate it using the code.
* The assets folder. Because this repository was build in order to make the code used to generate and wrangle the data used
in a scientific paper, the assets folder holds some third party data and other information.

If you have any doupt, don't exitate on contacting me.

## The Database

Those are the collumns in our database. Soon they will get a proper description.

| Field                                  | Type         | Null | Key | Default | Extra | Description |  
|---                                     | ---          | ---  | --- | ---     | ---   |---          |
| SIGLA_LEGENDA                          | varchar(200) | YES  |     | NULL    |       |             |
| NOME_CANDIDATO                         | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_DETALHE_SITUACAO_CANDIDATURA | varchar(200) | YES  |     | NULL    |       |             |
| SIGLA_UE                               | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_ELEICAO                         | varchar(200) | YES  |     | NULL    |       |             |
| NOME_COLIGACAO                         | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_SITUACAO_TOTAL_TURNO         | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_COR_RACA                        | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_PROTOCOLO_CANDIDATURA           | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_LEGENDA                         | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_OCUPACAO                     | varchar(200) | YES  |     | NULL    |       |             |
| ANO_ELEICAO                            | int(11)      | YES  |     | NULL    |       |             |
| DATA_NASCIMENTO                        | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_NACIONALIDADE                   | varchar(200) | YES  |     | NULL    |       |             |
| SIGLA_PARTIDO                          | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_TITULO_ELEITORAL_CANDIDATO      | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_ELEICAO                      | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_CARGO                        | varchar(200) | YES  |     | NULL    |       |             |
| NOME_SOCIAL_CANDIDATO                  | varchar(200) | YES  |     | NULL    |       |             |
| NOME_LEGENDA                           | varchar(200) | YES  |     | NULL    |       |             |
| SITUACAO_REELEICAO                     | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_SITUACAO_CANDIDATURA         | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_SEXO                         | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_ESTADO_CIVIL                    | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_CANDIDATO                       | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_PARTIDO                         | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAP_GRAU_INSTRUCAO               | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_MUNICIPIO_NASCIMENTO            | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_CPF_CANDIDATO                   | varchar(200) | YES  |     | NULL    |       |             |
| NOME_EMAIL                             | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_TIPO_ELEICAO                    | varchar(200) | YES  |     | NULL    |       |             |
| TIPO_ABRANGENCIA                       | varchar(200) | YES  |     | NULL    |       |             |
| COMPOSICAO_LEGENDA                     | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_UE                           | varchar(200) | YES  |     | NULL    |       |             |
| NOME_PARTIDO                           | varchar(200) | YES  |     | NULL    |       |             |
| IDADE_DATA_ELEICAO                     | varchar(200) | YES  |     | NULL    |       |             |
| NOME_UE                                | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_DETALHE_SITUACAO_CANDIDATURA    | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_ESTADO_CIVIL                 | varchar(200) | YES  |     | NULL    |       |             |
| SITUACAO_DECLARAR_BENS                 | varchar(200) | YES  |     | NULL    |       |             |
| SIGLA_UF_NASCIMENTO                    | varchar(200) | YES  |     | NULL    |       |             |
| DESPESA_MAX_CAMPANHA                   | varchar(200) | YES  |     | NULL    |       |             |
| SEQUENCIAL_COLIGACAO                   | varchar(200) | YES  |     | NULL    |       |             |
| IDADE_DATA_POSSE                       | varchar(200) | YES  |     | NULL    |       |             |
| SEQUENCIAL_CANDIDATO                   | varchar(200) | YES  |     | NULL    |       |             |
| HORA_GERACAO                           | varchar(200) | YES  |     | NULL    |       |             |
| NOME_TIPO_ELEICAO                      | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_GRAU_INSTRUCAO                  | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_SEXO                            | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_SITUACAO_TOTAL_TURNO            | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_TURNO                           | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_SITUACAO_CANDIDATURA            | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_CARGO                           | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_GRAU_INSTRUCAO               | varchar(200) | YES  |     | NULL    |       |             |
| SIGLA_UF                               | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_COR_RACA                     | varchar(200) | YES  |     | NULL    |       |             |
| NOME_URNA_CANDIDATO                    | varchar(200) | YES  |     | NULL    |       |             |
| NUMERO_PROCESSO                        | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_COMPOSICAO_COLIGACAO         | varchar(200) | YES  |     | NULL    |       |             |
| CODIGO_OCUPACAO                        | varchar(200) | YES  |     | NULL    |       |             |
| NOME_MUNICIPIO_NASCIMENTO              | varchar(200) | YES  |     | NULL    |       |             |
| TIPO_AGREMIACAO                        | varchar(200) | YES  |     | NULL    |       |             |
| DESCRICAO_NACIONALIDADE                | varchar(200) | YES  |     | NULL    |       |             |
| DATA_ELEICAO                           | varchar(200) | YES  |     | NULL    |       |             |
| DATA_GERACAO                           | varchar(200) | YES  |     | NULL    |       |             |

