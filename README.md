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
<p align="justify">A análise exploratória dos dados mostrou uma sazonalidade da influenza nesta população entre os meses de Março e Julho.  Embora tenha  ocorrido uma queda brusca no número de internações a partir de março de 2020 , foi encontrada uma correlação  fraca [ 0.59] entre o número de hospitalizações por influenza e o índice de isolamento social [p-valor=0.08].


# Vídeos do Projeto

 Vídeo da Proposta

 Vídeo da Apresentação Final
 
# Slides do Projeto

 Slides da Proposta
Link para slides de apresentação da proposta do projeto.

[*Slides da Apresentação Final*](https://docs.google.com/presentation/d/1s2u8UMjPYv8Wt1XQXc1LJa0I2yuEOJ-tSRMhBdDBJLs/edit?usp=sharing)

# Introdução e Referenciais de Teóricos

<p align="justify"> A gripe é uma doença aguda do sistema respiratório, causada pelo vírus Influenza, tendo alta capacidade de transmissão e distribuição global. A transmissão do vírus Influenza entre humanos ocorre pela via respiratória por meio de secreções como aerossóis, gotículas ou por contato direto da mucosa. São poucas as opções disponíveis para o seu controle. Dentre essas, a vacinação constitui a forma mais eficaz para o controle da doença e de suas complicações[1]. 
<p align="justify"> No Brasil, segundo dados obtidos pelo Projeto VigiGripe1, em 2003 verificou-se que a influenza apresentava pico de atividade entre os meses de maio e setembro, e que, no entanto casos, esporádicos eram detectados em outros meses do ano. O vírus apresenta altas taxas de mutação, o que resulta frequentemente na inserção de novas variantes virais na comunidade, para as quais a população não apresenta imunidade.1 A campanha de vacinação contra a influenza é alterada anualmente, com base nas recomendações da Organização Mundial da Saúde (OMS), tendo sido realizada no periodo de abril a maio, nos anos de 2015 a 2017[2,3,4] no periodo de abril a junho em 2018[5], de abril a maio em 2019[6], e entre os meses de março e maio em 2020[7]. 
<p align="justify"> Nascimento et. al (2020) avaliaram através de um estudo clínico transversal, a prevalência de hospitalizações por doenças respiratórias na infância, entre elas infecções respiratórias de vias aéreas superiores, asma / bronquite, bronquiolite e pneumonia, e o impacto do isolamento social por COVID-19 no comportamento sazonal dessas doenças. Os autores encontraram na redução inesperada do número de hospitalizações na população pediátrica durante este período, e concluíram que as medidas de isolamento social adotadas durante a pandemia COVID-19 podem ter interferido na sazonalidade dessas doenças respiratórias infantis[8]. 
 <p align="justify">  No Brasil, as crianças estiveram fora da pré-escola e de creches no ano de 2020, devido às adaptações necessárias ao enfrentamento da COVID-19.
Dessa forma, o distanciamento social, o uso de mascaras, a suspensão de aulas em escolas e os protocolos de enfrentamento adotados como medida de saúde pública para controlar a pandemia de COVID-19 podem ter afetado a incidência de hospitalizações por doenças respiratórias, como a gripe (influenza, CID 10 - J11). 
 <p align="justify"> Considerando a repercussão dessas experiências sociais únicas na saúde infantil, esse estudo tem como objetivo, através da ciência de dados, avaliar o impacto do distanciamento social em resposta à pandemia de COVID-19 em internações hospitalares de crianças por influenza.
 
# Perguntas de Pesquisa
<p align="justify">Qual o impacto do distanciamento social no Brasil em resposta à pandemia de COVID-19 na incidência de hospitalização de crianças por gripe (influenza)?</p>

 
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
> Indice de Isolamento Social | [*Indice-IPEA*](https://medidas-covidbr-iptsp.shinyapps.io/painel/) | <p align="justify"> O Indice de isolamento social foi criado pelo IPEA em parceria com o Ministério da Economia e UFG, a partir das medidas de isolamento social governamentais para enfrentamento da COVID-19</p>

> Qual o esquema/dicionário desse banco (o formato é livre)?
<p align="justify">É apresentado a partir de codebook em planilha.</p>

> O que descobriu sobre esse banco?
<p align="justify"> O indice de isolamento é uma série temporal, contruído com base nas medidas de isolamento decretadas por governos. O indice é "composto por seis variáveis: restrições a eventos e atividades culturais, esportivas ou religiosas; restrições ao funcionamento de bares e restaurantes; restrições ao comércio em geral; restrições sobre atividades industriais; suspensão de aulas; e restrições ao transporte terrestre, fluvial e marítimo de passageiros." (Moraes, RF, de, 2020 - IPEA)</p>

[*Moraes-2020*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35462&Itemid=4/)

Para saber mais sobre o indice de isolamento social, acesse Nota Técnica-2020-Maio-Número19 do IPEA [*Nota Técnica-2020-Maio-Número19-Dinte*](https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=35567).


> Quais as transformações e tratamentos (e.g., dados faltantes e limpeza) feitos?

Os dados foram extraidos a partir do seguinte [*link*](https://docs.google.com/spreadsheets/d/1a5_eloeGJkTWC6V4J39Qbbbm2wMPQlzcTeBxPy-hu80/edit#gid=0) disponibilizado pelo IPEA. A seguir foi realizada:

- Preparação de dados a partir de análises de tipos de dados e reconfigurações/conversões de datas.

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

# Análises Realizadas
> Descrição detalhada das análises realizadas.
>
>
>
>Relate aqui também a evolução do projeto: possíveis problemas enfrentados e possíveis mudanças de trajetória. Relatar o processo para se alcançar os resultados é tão importante quanto os resultados.
>
>
>
> Nesta seção ou na seção de Resultados podem aparecer destaques de código como indicado a seguir. Note que foi usada uma técnica de highlight de código, que envolve colocar o nome da linguagem na abertura de um trecho com `~~~`, tal como `~~~python`.
>
> Os destaques de código devem ser trechos pequenos de poucas linhas, que estejam diretamente ligados a alguma explicação. Não utilize trechos extensos de código. Se algum código funcionar online (tal como um Jupyter Notebook), aqui pode haver links. No caso do Jupyter, preferencialmente para o Binder abrindo diretamente o notebook em questão.

~~~python
df = pd.read_excel("/content/drive/My Drive/Colab Notebooks/dataset.xlsx");
sns.set(color_codes=True);
sns.distplot(df.Hemoglobin);
plt.show();
~~~

## Ferramentas
> Panorama das ferramentas utilizadas incluindo discussão sobre o uso das mesmas

# Resultados
> Descrição dos resultados mais importantes obtidos.
>
> Apresente os resultados da forma mais rica possível, com gráficos e tabelas. Mesmo que o seu código rode online em um notebook, copie para esta parte a figura estática. A referência a código e links para execução online pode ser feita aqui ou na seção de Análises Realizadas (o que for mais pertinente).

# Discussão
> Discussão dos resultados. Relacionar os resultados com as perguntas de pesquisa ou hipóteses avaliadas.
>
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
> Lista de artigos, links e referências bibliográficas.
>
> Fiquem à vontade para escolher o padrão de referenciamento preferido pelo grupo.
