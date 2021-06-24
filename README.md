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

<p align="justify">O distanciamento social como medida de saúde pública para controlar a pandemia de COVID-19 pode ter afetado o fardo de outras doenças respiratórias, tendo, desta forma, impactado na incidência de hospitalizações por doenças respiratórias com sazonalidade conhecida, como a gripe (influenza, CID 10 - J11).
<p align="justify">Desta forma, esse estudo teve  como objetivo avaliar o impacto do distanciamento social em resposta à pandemia de COVID-19 em internações hospitalares por influenza, entre os anos de 2015 a 2020, através de uma análise de série temporal.
<p align="justify">Os dados referentes às internações foram obtidos na plataforma DATA SUS, e os dados referentes ao índice de isolamento social na Brasil foram obtidos na base Ipea - Instituto de Pesquisa Econômica Aplicada.
<p align="justify">A análise exploratória dos dados mostrou uma sazonalidade da influenza nesta população entre os meses de Março e Julho.  Embora tenha  ocorrido uma queda brusca no número de internações a partir de março de 2020 , foi encontrada uma correlação  fraca [ρ= 0.59] entre o número de hospitalizações por influenza e o índice de isolamento social [p=0.08]. Para o futuro, esta pesquisa poderá se dirigir à busca de novas variáveis que possam ter vindo a interferir individualmente ou em conjunto ao isolamento social, para promover a redução dos casos de internação por influenza em crianças de 0 a 4 anos, observada em 2020. 


# Vídeos do Projeto
[*Vídeo de Apresentação do Projeto*](https://drive.google.com/file/d/1Ncb4lrw9qq2EVpo1PS115lLMc4epxSyP/view?usp=sharing)

[*Vídeo da Apresentação Final*](https://youtu.be/X_k6-WSSHGo)
 
# Slides da Apresentação Final
[*Slides da Apresentação Final*](https://docs.google.com/presentation/d/1s2u8UMjPYv8Wt1XQXc1LJa0I2yuEOJ-tSRMhBdDBJLs/edit?usp=sharing)

# Introdução e Referenciais de Teóricos

<p align="justify"> A gripe é uma doença aguda do sistema respiratório, causada pelo vírus Influenza, tendo alta capacidade de transmissão e distribuição global. A transmissão do vírus Influenza entre humanos ocorre pela via respiratória por meio de secreções como aerossóis, gotículas ou por contato direto da mucosa. São poucas as opções disponíveis para o seu controle. Dentre essas, a vacinação constitui a forma mais eficaz para o controle da doença e de suas complicações[1]. 
<p align="justify"> No Brasil, segundo dados obtidos pelo Projeto VigiGripe1, em 2003 verificou-se que a influenza apresentava pico de atividade entre os meses de maio e setembro, e que, no entanto casos, esporádicos eram detectados em outros meses do ano. O vírus apresenta altas taxas de mutação, o que resulta frequentemente na inserção de novas variantes virais na comunidade, para as quais a população não apresenta imunidade.1 A campanha de vacinação contra a influenza é alterada anualmente, com base nas recomendações da Organização Mundial da Saúde (OMS), tendo sido realizada no periodo de abril a maio, nos anos de 2015 a 2017[2,3,4] no periodo de abril a junho em 2018[5], de abril a maio em 2019[6], e entre os meses de março e maio em 2020[7]. 
<p align="justify"> Nascimento et. al (2020) avaliaram através de um estudo clínico transversal, a prevalência de hospitalizações por doenças respiratórias na infância, entre elas infecções respiratórias de vias aéreas superiores, asma / bronquite, bronquiolite e pneumonia, e o impacto do isolamento social por COVID-19 no comportamento sazonal dessas doenças. Os autores encontraram na redução inesperada do número de hospitalizações na população pediátrica durante este período, e concluíram que as medidas de isolamento social adotadas durante a pandemia COVID-19 podem ter interferido na sazonalidade dessas doenças respiratórias infantis[8]. 
 <p align="justify">  No Brasil, as crianças estiveram fora da pré-escola e de creches no ano de 2020, devido às adaptações necessárias ao enfrentamento da COVID-19.
Dessa forma, o distanciamento social, o uso de mascaras, a suspensão de aulas em escolas e os protocolos de enfrentamento adotados como medida de saúde pública para controlar a pandemia de COVID-19 podem ter afetado a incidência de hospitalizações por doenças respiratórias, como a gripe (influenza, CID 10 - J11). 
 <p align="justify"> Considerando a repercussão dessas experiências sociais únicas na saúde infantil, esse estudo tem como objetivo, através da ciência de dados, avaliar o impacto do distanciamento social em resposta à pandemia de COVID-19 em internações hospitalares de crianças por influenza.
 
# Pergunta de Pesquisa
<p align="justify">Qual o impacto do distanciamento social no Brasil em resposta à pandemia de COVID-19 na incidência de hospitalização de crianças por gripe (influenza)?</p>

 
## Hipótese
<p align="justify">Houve redução na incidência de hospitalizações por influenza em crianças de 0 a 4 anos, em decorrência do distanciamento social em resposta à pandemia de COVID-19.</p>

## População estudada
Crianças de 0 a 4 anos.

## Período observado
2015 a 2020.

## Critérios de inclusão 
<p align="justify"> Crianças de 0 a 4 anos, internadas em decorrência da Influenza no Serviço Único de Saúde (SUS) do Brasil, no período de 2015 a 2020.</p>

# Bases de Dados e Evolução

## Bases Estudadas e Adotadas

> Base de Dados | Endereço na Web | Resumo descritivo
> -- | -- | --
> SIH - DATASUS | [*SIH-DATASUS*](http://www2.datasus.gov.br/DATASUS/index.php?area=0203&id=6926) | <p align="justify">O Sistema de Informações Hospitalares - SIH, registra dados de todos os atendimentos provenientes de internações hospitalares que foram financiadas pelo SUS. Mensalmente, estes dados são disponibilizados como OpenData para acesso via DATASUS. Para mais informações acesse a [*wiki-DATASUS*](https://wiki.saude.gov.br/sih/index.php/P%C3%A1gina_principal)</p>

> Qual o esquema/dicionário desse banco?
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
> Indice de Isolamento Social | [*Indice-IPEA*](https://medidas-covidbr-iptsp.shinyapps.io/painel/) | <p align="justify"> O Indice de isolamento social foi criado pelo IPEA em parceria com o Ministério da Economia e UFG, a partir das medidas de isolamento social governamentais para enfrentamento da COVID-19</p>

> Qual o esquema/dicionário desse banco (o formato é livre)?
<p align="justify">É apresentado a partir de codebook em planilha.</p>

> O que descobriu sobre esse banco?
<p align="justify"> O indice de isolamento é uma série temporal, construída com base nas medidas de isolamento decretadas por governos. O indice é "composto por seis variáveis: restrições a eventos e atividades culturais, esportivas ou religiosas; restrições ao funcionamento de bares e restaurantes; restrições ao comércio em geral; restrições sobre atividades industriais; suspensão de aulas; e restrições ao transporte terrestre, fluvial e marítimo de passageiros." (Moraes, RF, de, 2020 - IPEA)</p>

[*Moraes-2020*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35462&Itemid=4/)

Para saber mais sobre o indice de isolamento social, acesse Nota Técnica-2020-Maio-Número19 do IPEA [*Nota Técnica-2020-Maio-Número19-Dinte*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35567).


> Quais as transformações e tratamentos (e.g., dados faltantes e limpeza) feitos?

Os dados foram extraidos a partir do seguinte [*link*](https://docs.google.com/spreadsheets/d/1a5_eloeGJkTWC6V4J39Qbbbm2wMPQlzcTeBxPy-hu80/edit#gid=0) disponibilizado pelo IPEA. A seguir foi realizada:

- Preparação de dados a partir de análises de tipos de dados e reconfigurações/conversões de datas.

> Apresente aqui uma Análise Exploratória (inicial) sobre esta base.

A análise exploratória inicial foi realizada em um notebook executável e pode ser acessada no link a seguir:

[*Analise Exploratória*](https://colab.research.google.com/drive/15yIhW_BfnWs5OOBj1EyC9R7L3YGWI04B?usp=sharing)

## Integração entre Bases e Análise Exploratória

A integração entre os datasets extraidos do DATASUS, por ano, foi a partir da soma dos números de casos por mês, tendo em vista que o layout dos datasets é pre-processado de forma idêntica. Para este processo foi realizada soma e transposição linha versus coluna dos dados via excel.

Para permitir a realização da correlação entre as séries temporais de isolamento social com os dados do DATASUS em 2020, foi necessário realizar a transformação do índice diário de isolamento em um índice mensal, a partir da média das porcentagens diárias de isolamento.   

# Metodologia
A metodologia utilizada será baseada em KDD.

# Ferramentas
Python, Bibliotecas Pandas, Numpy, Statistics, Matplotlib, Excel e o Google Colab;

# Cronograma
[*Cronograma*](https://docs.google.com/document/d/19WYZ1MMnKAfzT6nPk9wERh0kRPu2wLS0aIIbGzgJ2CM/edit?usp=sharing)

# Análises Realizadas

<p align="justify"> A partir da obtenção, pré-processamento e integração dos dados do SIH-DATASUS e do IPEA, iniciou-se a análise exploratória dos dados, os quais, estavam organizados em séries temporais(ST). Nesta perspectiva, foi necessário compreender as particularidades deste sub-domínio estatístico vasto das ST, que inclui a importância dos processos de conversões de datas, decomposição da ST em tendência, sazonalidade e residual, análise de estacionariedade, autocorrelação e dependendo do contexto estudado, o uso de modelos preditivos de autoregressão e suas variações(AR, ARMA, ARIMA). </p>
 
<p align="justify"> A análise exploratória foi desenvolvida em um notebook colab com Python e bibliotecas para ciência de dados (pandas, numpy, matplotlib, scipy, seaborn, datetime, statsmodels e dentre outras) e com excel para realizar parte do pré-processamento. A análise exploratória dividiu-se em 4 partes: </p>

 1) DATASUS - Importação, Pré-Processamento e Visualização dos dados;
 2) Indice de Isolamento Social no Brasil 2020-2021 - Importação, Pré-Processamento e Visualização dos dados;
 3) Correlação entre Séries Temporais;
 4) Conclusões.

<p align="justify"> Na primeira etapa, realizamos a importação dos .csv do DATASUS, os quais já haviam passado por uma etapa do pré-processamento, usando a ferramenta excel, para a limpeza de metadados, integração e transposições, realizadas em mais de 6 testes distintos, a fim de verificar o melhor formato para importação dos dados no notebook. Em seguida, já com os dados importados no notebook, foi realizada outra etapa de pré-processamento, envolvendo entendimento dos tipos de dados do dataset e conversões de data. A próxima análise desta etapa envolveu a visualização de dados, com o desenvolvimento de gráficos da série temporal completa e Gráfico de sobreposição das séries temporais. </p>
 
<p align="justify"> Ainda na primeira etapa, foi realizada a análise estatística da serie temporal DATASUS, iniciando pela verificação de estacionariedade, decomposição da série temporal e desenvolvimento de gráficos de autocorrelação.</p>
 
<p align="justify"> Na segunda etapa, realizamos a importação dos dados crus no notebook, em .csv, e realizamos conversões de data. Em seguida realizamos a visualização de dados, teste de estacionariedade, decomposição da série temporal e autocorrelação.</p>
 
<p align="justify"> Na terceira etapa, foi realizada a análise de normalidade das séries com Shapiro-Wilk e análise de correlação entre as duas séries temporais utilizando Spearman, tendo em vista que os dados de 2020 do DATASUS foram testados como normais e o indice de isolamento como não-normal.</p>

<p align="justify"> Na etapa de conclusão foram interpretados os resultados, apresentando os futuros direcionamentos do estudo.</p>

<p align="justify"> Após compreender a correlação entre as séries temporais, foi decidido como próximo direcionamento do projeto, desenvolver um modelo preditivo, usando ARIMA, para verificar se, conforme a sazonalidade e tendência de internações de 2015 a 2019, a curva de 2020, prevista pelo modelo, seria a mesma que a curva real observada. Se fossem iguais, isso poderia indicar que o número de internações tendia a se comportar da forma com foi observada, por tendencia e sazonalidade natural da ST. Porém, se fossem diferentes, seria mais um dado para corroborar com a comprovação de que uma ou mais variáveis interferiram na curva observada em 2020.</p>

<p align="justify"> Em relação a evolução do projeto, houveram duas mudanças de trajetória importantes a serem citadas. A primeira é que a metodologia inicial de desenvolvimento foi o CRISP-DM. Porém, no decorrer do projeto, entendeu-se que toda a documentação proposta como padrão no Git seguia uma visão mais voltada para metodologia KDD. Com isso, para evitar a duplicidade de metodologias e redundância de documentação, foi resolvido utilizar somente a metodologia KDD.</p>

<p align="justify"> A segunda mudança de trajetória foi em relação a análise de mortalidade por influenza na mesma faixa etária e sua correlação com o indice de isolamento. Nesta quesito, após a coleta inicial de dados, notou-se inicialmente a incidência de dados faltantes e em seguida houve a hipótese de viés nos dados disponibilizados. O viés se relacionou à baixissima quantidade de casos de mortalidade em um indice nacional, chegando a 1 em alguns meses. Nesta perspectiva, foi decidido não estudar tal fenomêno no momento, deixando para compreender tais complexidades, possiveis viéses e dentre outras especificidades em um projeto separado ou em um momento futuro. </p> 

## Ferramentas
<p align="justify"> Como ferramentas, foram utilizadas o notebook Google Colab, com python, por ser uma ferramenta online com capacidade de colaboração entre os membros da equipe. A linguagem python foi escolhida por ser uma linguagem muito utilizada atualmente, facilitando a resolução problemas, por haver ambientes de discussão entre a comunidade e documentação oficial bem atualizadas. Como complemento, em apoio à realização de atividades de pré-processamento, foi utilizado o excel, por facilitar o processo de testes e realização de alterações facilmente visualizaveis. </p>  

# Resultados
<p align="justify"> O principal resultado obtido foi o da correlação e p-valor(two-sided) entre o numero de casos de internações por influenza em crianças de 0 a 4 anos em 2020 e o indice de isolamento social em decorrencia da covid-19. Os resultados das análises indicaram uma correlação de spearman intermediária (0,58), sem significância estatistica (0,08), o qual responde a pergunta de pesquisa definida.</p>

<p align="justify"> Em seguida, o resultado mais importante foi o entendimento que, apesar do isolamento mostrar-se estatisticamente insignificante para responder a pergunta, houve o levantamento de indícios que uma ou mais variáveis interferiram na redução das internações por influenza na faixa de 0 a 4 anos. Apesar das variáveis não terem sido identificadas neste momento, tal fenonomeno começa a ser comprovado pelo desenvolvimento do gráfico de sobreposição das séries temporais, onde a modificação de comportamento da série pode ser claramente observado em 2020, em relação a 2015 a 2019, conforme a figura abaixo. </p>

![imagem0](https://github.com/raphaelgoncalves/UNICAMP-DataSci4Health-Projeto-Final/blob/main/Assets/imagem0.PNG)
Figura 1: Gráfico de sobreposição das séries temporais

<p align="justify"> Outro resultado importante foi o de comparação entre a curva do modelo preditivo ARIMA e a curva real de internações em 2020, mostrando-se completamente diferentes, conforme podemos observar na figura abaixo.</p>

![imagem1](https://github.com/raphaelgoncalves/UNICAMP-DataSci4Health-Projeto-Final/blob/main/Assets/imagem1.PNG)

<p align="justify"> Além do escopo proposto para esta pesquisa, pode-se observar, com base na literatura estudada, dados de sazonalidade diferentes dos apresentados na literatura para a influenza no Brasil, em até 2 meses de diferença.</p>

# Discussão
> Discussão dos resultados. Relacionar os resultados com as perguntas de pesquisa ou hipóteses avaliadas.

<p align="justify"> O principal resultado obtido foi que a hipótese nula definida foi negada, a partir da correlação e p-valor(two-sided) entre o numero de casos de internações por influenza em crianças de 0 a 4 anos em 2020 e o indice de isolamento social em decorrencia da covid-19. Os resultados das análises indicaram um </p>

<p align="justify"> Em seguida, os resultados secundários foram a comprovação que houve uma alteração de na curva da série temporal

> A discussão dos resultados também pode ser feita opcionalmente na seção de Resultados, na medida em que os resultados são apresentados. Aspectos importantes a serem discutidos: É possível tirar conclusões dos resultados? Quais? Há indicações de direções para estudo? São necessários trabalhos mais profundos?

# Conclusão
> Destacar as principais conclusões obtidas no desenvolvimento do projeto.
>
> Destacar os principais desafios enfrentados.
>
> Principais lições aprendidas.

# Trabalhos Futuros
> O que poderia ser melhorado se houvesse mais tempo?

# Referências Bibliográficas
> 1-	FORLEO-NETO, E. et al. Influenza.  Rev Soc Bras Med Trop, Uberaba, v. 36, n. 2, p. 267-274, 2003.

> 2-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2015. Disponível em: http://portalarquivos.saude.gov.br/images/pdf/2015/marco/30/Informe-Cp-Influenza---25-03-2015-FINAL.pdf

> 3-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2016. Disponível em: https://sbim.org.br/images/files/informe_cp_influenza-_11_03_2016_final.pdf

> 4-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2017. Disponível em: https://www.prefeitura.sp.gov.br/cidade/secretarias/upload/chamadas/resumo_operacional_campanha_vacinacao_contra_influenza_2017_1493734874.pdf

> 5-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2018. Disponível em: https://portalarquivos2.saude.gov.br/images/pdf/2018/abril/18/Informe-Cp-Influenza---01-03-2018-Word-final-28.03.18%20final.pdf

> 6-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2019. Disponível em: https://portalarquivos2.saude.gov.br/images/pdf/2019/fevereiro/28/Informe-Cp-Influenza-28-02-2019-final.pdf

> 7-	Ministério da Saúde. Informe Técnico. Campanha Nacional de Vacinação contra a Influenza, 2020. Disponível em: https://www.saude.go.gov.br/files/imunizacao/influenza/InformeTecnicoInfluenza.2020.pdf

> 8-	Nascimento MS, Baggio DM, Fascina LP, do Prado C. Impact of social isolation due to COVID-19 on the seasonality of pediatric respiratory diseases. PLoS One. 2020 Dec 11;15(12):e0243694. doi: 10.1371/journal.pone.0243694. Disponível em: https://pubmed.ncbi.nlm.nih.gov/33306735/

