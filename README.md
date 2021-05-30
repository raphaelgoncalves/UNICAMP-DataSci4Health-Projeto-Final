# <p align="justify"> O impacto do distanciamento social em resposta à pandemia de COVID-19 e as internações hospitalares por influenza em crianças no Brasil.</p>
# <p align="justify"> The impact of social distance in response to the COVID-19 pandemic and hospitalizations for influenza in children in Brazil.</p>

# Apresentação

O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação [*Ciência e Visualização de Dados em Saúde*](https://github.com/datasci4health/home), oferecida no primeiro semestre de 2021, na Unicamp.


> |Nome  | RA | Especialização|
> |--|--|--|
> | Aline Priscila Souza | 231612 | Fisioterapia|
> | Brayan Crispiano Ksenhuck | 165192 | Engenharia Elétrica|
> | Edmar Rodrigues Filho  | 166690 | Engenharia Elétrica|
> | José Mario Alves Júnior | 216818 | Biomedicina|
> | Raphael de Paiva Gonçalves  | 234839  | Ciência da Computação|


# Descrição Resumida do Projeto
<p align="justify">O distanciamento social como medida de saúde pública para controlar a pandemia de COVID-19 pode ter afetado o fardo de outras doenças respiratórias, tendo, desta forma, impactado na incidência de hospitalizações por doenças respiratórias, como a gripe (influenza, CID 10 - J11).</p>
  
<p align="justify">A epidemiologia do vírus influenza é bem conhecida nas regiões Sul e Sudeste do Brasil, onde a sazonalidade está bem caracterizada, ocorrendo nos meses de outono e inverno, especialmente nos meses de maio a julho, no entanto casos esporádicos podem ser detectados em outros meses do ano.</p>

<p align="justify">No Brasil, as crianças estiveram fora da pré-escola e de creches no ano de 2020, devido às adaptações necessárias ao enfrentamento da Covid-19. Considerando a repercussão dessas experiências sociais únicas na saúde infantil, esse estudo tem como objetivo, através da ciência de dados, avaliar o impacto do distanciamento social em resposta à pandemia de COVID-19 em internações hospitalares por influenza. Para isso, será utilizada a metodologia KDD, com ferramentas de Python, com 2 datasets de opendata disponibilizado pelo governo federal do Brasil, Datasus.</p>

## Hipótese
<p align="justify">Houve redução na incidência de hospitalizações por influenza em crianças de 0 a 4 anos, em decorrência do distanciamento social em resposta à pandemia de COVID-19.</p>

## População estudada
Crianças de 0 a 4 anos.

## Período observado
2015 a 2020.

## Critérios de inclusão 
<p align="justify"> Crianças de 0 a 4 anos, internadas em decorrência da Influenza no Serviço Único de Saúde (SUS) do Brasil, no período de 2015 a 2020.</p>

## Vídeo de apresentação
[*Vídeo de Apresentação do Projeto*](https://drive.google.com/file/d/1Ncb4lrw9qq2EVpo1PS115lLMc4epxSyP/view?usp=sharing)

# Perguntas de Pesquisa
<p align="justify">Qual o impacto do distanciamento social no Brasil em resposta à pandemia de COVID-19 na incidência de hospitalização de crianças por gripe (influenza)?</p>

# Bases de Dados e Evolução

## Bases Estudadas e Adotadas

> Base de Dados | Endereço na Web | Resumo descritivo
> -- | -- | --
> SIH - DATASUS | [*SIH-DATASUS*](http://www2.datasus.gov.br/DATASUS/index.php?area=0203&id=6926) | <p align="justify">O Sistema de Informações Hospitalares - SIH, registra dados de todos os atendimentos provenientes de internações hospitalares que foram financiadas pelo SUS. Mensalmente, estes dados são disponibilizados como OpenData para acesso via DATASUS. Para mais informações acesse a [*wiki-DATASUS*](https://wiki.saude.gov.br/sih/index.php/P%C3%A1gina_principal)</p>

> Qual o esquema/dicionário desse banco (o formato é livre)?
<p align="justify">O SIH - DATASUS não disponibiliza um arquivo específico com o dicionário dos dados, porém os metadados são inseridos no dataset. </p>

> O que descobriu sobre esse banco?
<p align="justify">Devido ao fato do banco tratar de informações necessárias para a execução de pagamentos financeiros, a base tem um processo de atualização bem definido e constante. Em contato com os Administradores responsáveis pelos dados, o Núcleo de Informações da Atenção à Saúde, do Ministério da Saúde, confirmamos que os dados não são consolidados e podem ter alterações em seus registros em até 12 meses após o mês de referência, por exemplo, os dados de Janeiro/2020 podem ser atualizados até Dezembro/2020, sendo após este periodo, considerados consolidados. Para fins de acesso os dados do DataSus são disponibilizados via Tabwin, uma ferramenta que gera views de grandes datasets, a partir de filtros via interface gráfica.</p>

> Quais as transformações e tratamentos (e.g., dados faltantes e limpeza) feitos?

Inicialmente, cabe ressaltar que os dados já vieram pré-processados, pois os dados deste estudo são provenientes do Tabwin do DataSus. 
 - Limpeza de dados a partir da extração de metadados que estavam junto aos .csv dos datasets;
 - Preparação de dados a partir de reconfigurações de datas;
 - Preparação de dados a partir da transposição das  features linhas em colunas no .csv para gerar um data frame;
 - Preparação dos dados a partir da mudança da separação por ";" no dataset .csv para ",".


> Base de Dados | Endereço na Web | Resumo descritivo
> -- | -- | --
> Indice de Isolamento Social | [*Indice-IPEA*](https://medidas-covidbr-iptsp.shinyapps.io/painel/) | <p align="justify">O Indice de isolamento social foi criado pelo IPEA em parceria com o Ministério da Economia e UFG, a partir das medidas de isolamento social governamentais para enfrentamento da COVID-19</p>

> Qual o esquema/dicionário desse banco (o formato é livre)?
<p align="justify">É apresentado a partir de codebook em planilha.</p>

> O que descobriu sobre esse banco?
<p align="justify"> O indice de isolamento é uma série temporal, contruído com base nas medidas de isolamento decretadas por governos. O indice é "composto por seis variáveis: restrições a eventos e atividades culturais, esportivas ou religiosas; restrições ao funcionamento de bares e restaurantes; restrições ao comércio em geral; restrições sobre atividades industriais; suspensão de aulas; e restrições ao transporte terrestre, fluvial e marítimo de passageiros." (Moraes, RF, de, 2020 - IPEA)</p>

[*Moraes-2020*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35462&Itemid=4/)

Para saber mais sobre o indice de isolamento social, acesse Nota Técnica-2020-Maio-Número19 do IPEA [*Nota Técnica-2020-Maio-Número19-Dinte*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35567).


> Quais as transformações e tratamentos (e.g., dados faltantes e limpeza) feitos?
Os dados foram extraidos a partir do seguinte [*link*](https://docs.google.com/spreadsheets/d/1a5_eloeGJkTWC6V4J39Qbbbm2wMPQlzcTeBxPy-hu80/edit#gid=0) disponibilizado pelo IPEA. A seguir foi realizada: 
 A Preparação de dados a partir de análises de tipos de dados e reconfigurações/conversões de datas.

> Apresente aqui uma Análise Exploratória (inicial) sobre esta base.

A análise exploratória inicial foi realizada em um notebook executável e pode ser acessada no link a seguir:

[*Analise Exploratória*](https://colab.research.google.com/drive/15yIhW_BfnWs5OOBj1EyC9R7L3YGWI04B?usp=sharing)

## Integração entre Bases e Análise Exploratória

A integração entre os datasets foi a partir da soma dos números de casos por mês, tendo em vista que o layout dos datasets é pre-processado de forma idêntica. Para este processo foi realizada soma e transposição linha versus coluna dos dados via excel.

# Metodologia
A CRISP-DM não será mais utilizada, pois iria gerar redundância de documentação do projeto com esta documentação para as entregas, baseada em KDD.

# Ferramentas
Python, Bibliotecas Pandas, Numpy, Statistics, Matplotlib, Excel e o Google Colab;

# Cronograma
[*Cronograma*](https://docs.google.com/document/d/19WYZ1MMnKAfzT6nPk9wERh0kRPu2wLS0aIIbGzgJ2CM/edit?usp=sharing)
