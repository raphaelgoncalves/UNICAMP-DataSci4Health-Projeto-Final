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

<p align="justify">No Brasil, as crianças estiveram fora da pré-escola e de creches no ano de 2020, devido às adaptações necessárias ao enfrentamento da Covid-19. Considerando a repercussão dessas experiências sociais únicas na saúde infantil, esse estudo tem como objetivo, através da ciência de dados, avaliar o impacto do distanciamento social em resposta à pandemia de COVID-19 em internações hospitalares por influenza. Para isso, será utilizada a metodologia CRISP-DM, com ferramentas de Python, com um dataset de opendata disponibilizado pelo governo federal do Brasil, Datasus.</p>

## Hipótese
<p align="justify">Houve redução na incidência de hospitalizações e a mortalidade por influenza em crianças de 0 a 4 anos, em decorrência do distanciamento social em resposta à pandemia de COVID-19.</p>

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
<p align="justify">Qual o impacto do distanciamento social no Brasil em resposta à pandemia de COVID-19 na mortalidade hospitalar de crianças por gripe (influenza)?</p>

# Bases de Dados e Evolução
> Elencar bases de dados estudadas e/ou utilizadas no projeto, organizando em duas partes. Primeiro aquelas que foram estudadas, mas não serão usadas e em seguida as bases adotadas.

## Bases Estudadas e Adotadas

> Para cada base, coloque uma mini-tabela no modelo a seguir e depois detalhamento sobre como ela foi analisada/usada, conforme exemplo a seguir.

Base de Dados | Endereço na Web | Resumo descritivo
----- | ----- | -----
SIH - DATASUS | [*SIH-DATASUS*](http://www2.datasus.gov.br/DATASUS/index.php?area=0203&id=6926) | <p align="justify">A finalidade inicial do Sistema de Informações Hospitalares - SIH foi a de controle administrativo-financeiro para pagamento aos serviços hospitalares contratados pelo Instituto Nacional de Assistência Médica e Previdência Social(INAMPS). Para mais informações acesse a [*wiki-DATASUS*](https://wiki.saude.gov.br/sih/index.php/P%C3%A1gina_principal)</p>

> Faça uma descrição sobre o que concluiu sobre esta base. Sugere-se que respondam perguntas ou forneçam informações indicadas a seguir:
> * Qual o esquema/dicionário desse banco (o formato é livre)?
> * O que descobriu sobre esse banco?
> * Quais as transformações e tratamentos (e.g., dados faltantes e limpeza) feitos?
> * Apresente aqui uma Análise Exploratória (inicial) sobre esta base.

## Integração entre Bases e Análise Exploratória

> Descreva etapas de integração de fontes de dados e apresente a seguir uma análise exploratória que envolva ambas.

[*DataSUS*](http://www2.datasus.gov.br/DATASUS/index.php?area=02)
> Epidemiológicas e Morbidade > Geral, por local de internação - a partir de 2008 > Abrangencia Geográfica: Brasil por região e unidade da federação > Linha: Faixa Etária 1 > Coluna: Ano/mes atendimento > Conteúdo: Internações > Selecionar o Periodo > Lista Morb CID-10: Influenza > Faixa Etária 1: Escolher faixa etária

# Metodologia
CRISP-DM

# Ferramentas
Python, Bibliotecas Pandas, Numpy, Statistics, Matplotlib e o Google Colab;

# Cronograma
[*Cronograma*](https://docs.google.com/document/d/19WYZ1MMnKAfzT6nPk9wERh0kRPu2wLS0aIIbGzgJ2CM/edit?usp=sharing)
