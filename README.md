**Projeto:** Grupo 1 - House Price

**Problema de Negócio:**

O setor imobiliário ocupa um papel estratégico na economia brasileira, refletindo diretamente nas transformações econômicas e sociais do país. Apesar de sua importância, a precificação adequada ainda é um ponto sensível, especialmente diante das variações regionais e das múltiplas características que afetam o valor de uma propriedade (De Lucena, 2024).

Uma pesquisa realizada pelo Datafolha em parceria com o QuintoAndar (2024) destaca que um em cada três proprietários brasileiros tem dificuldades para definir o preço de venda ou aluguel de seus imóveis. A principal barreira identificada é a ausência de informações confiáveis sobre os valores praticados no mercado. Além disso, 65% dos brasileiros já desistiram de fechar um contrato por receio de estarem pagando ou cobrando um valor inadequado.

Além disso, de acordo com a pesquisa, a **definição incorreta do preço pode gerar impactos negativos**:

- **Valores elevados demais** afastam interessados;
- **Valores abaixo do ideal** resultam em prejuízos financeiros para proprietários e corretoras.

O método tradicional de avaliação, por ser manual e muitas vezes subjetivo, tende a ser lento e suscetível a erros, comprometendo a eficiência e a competitividade do setor. Diante desse cenário, a adoção de um modelo preditivo baseado em dados surge como uma solução promissora. Ao automatizar o processo de precificação, é possível alcançar maior precisão, reduzir o tempo de avaliação e apoiar decisões mais estratégicas. Isso se traduz em ganhos comerciais, melhor experiência para o cliente e uma atuação mais assertiva no mercado.

**Objetivos:** 

Prever o preço de imóveis com base em características estruturais e geográficas.

**Stakeholders:**  

Corretora

# Detalhes do Dataset de Imóveis de Ames

## Descrição Geral
O conjunto de dados contém informações detalhadas sobre propriedades residenciais vendidas em Ames, Iowa, entre 2006 e 2010. Ele inclui 80 variáveis explicativas (quantitativas e qualitativas) que descrevem características físicas, localização, condições de venda e outros atributos relevantes dos imóveis.

## Estrutura dos Dados
- **Número de observações**: ~1,460 propriedades
- **Número de variáveis**: 80 (79 features + 1 target)
- **Variável alvo**: `SalePrice` (preço de venda do imóvel)

## Principais Categorias de Variáveis

### 1. Características Físicas
| Variável | Descrição | Tipo |
|----------|-----------|------|
| `LotArea` | Tamanho do lote em pés quadrados | Numérico |
| `GrLivArea` | Área habitável acima do nível do solo | Numérico |
| `Bedroom` | Número de quartos acima do nível do solo | Inteiro |
| `FullBath` | Número de banheiros completos | Inteiro |
| `HalfBath` | Número de banheiros parciais | Inteiro |
| `YearBuilt` | Ano de construção original | Inteiro |
| `YearRemodAdd` | Ano de reforma | Inteiro |

### 2. Qualidade e Condição
| Variável | Escala | Descrição |
|----------|--------|-----------|
| `OverallQual` | 1-10 | Avaliação geral de material e acabamento |
| `OverallCond` | 1-10 | Avaliação geral da condição do imóvel |
| `KitchenQual` | Ex,Gd,TA,Fa,Po | Qualidade da cozinha |
| `BsmtQual` | Ex,Gd,TA,Fa,Po,NA | Qualidade do porão |

### 3. Localização
| Variável | Valores | Descrição |
|----------|---------|-----------|
| `Neighborhood` | 25 categorias | Bairros de Ames |
| `MSZoning` | A,C,FV,I,RH,RL,RP,RM | Zoneamento |
| `Condition1` | 9 categorias | Proximidade a vias/ferrovias |

### 4. Detalhes de Venda
| Variável | Descrição | Tipo |
|----------|-----------|------|
| `SaleType` | Tipo de transação | Categórico |
| `SaleCondition` | Condição da venda | Categórico |
| `YrSold` | Ano da venda | Inteiro |
| `MoSold` | Mês da venda | Inteiro |

## Aplicações Típicas
- 🏠 **Previsão de preços** de imóveis
- 📊 **Análise de mercado** imobiliário
- 🔍 Identificação de **fatores valorizantes**
- 🧠 **Benchmark** para modelos de machine learning

## Dicionário Completo
O arquivo [data_description.txt](data_description.txt) contém a descrição detalhada de todas as variáveis disponíveis no dataset.

## Observações Importantes
- Contém tanto variáveis numéricas quanto categóricas
- Alguns valores podem estar ausentes (NA)
- Ideal para praticar:
  - Análise exploratória (EDA)
  - Tratamento de dados faltantes
  - Feature engineering
  - Modelagem preditiva


Link Kanban:https://almeidadatasciencehouseprice.atlassian.net/jira/software/projects/KAN/boards/1?atlOrigin=eyJpIjoiMTZmODM5NzY3YmUxNDQ5OWE0MGM5YmZlN2VhMTlmNjAiLCJwIjoiaiJ9

Link Google Colab: https://colab.research.google.com/drive/145ehe7XaVXsqbgGRKWbf3YsJoCya33Z9?usp=sharing

**Referências:**
1. DE LUCENA, João Gilberto Rocha Batista et al. Precificação de lançamentos imobiliários em Goiânia. 2024.
2. QuintoAndar/Datafolha: 65% dos brasileiros deixaram de negociar imóvel pelo preço, diz estudo. Disponível em: <https://economia.uol.com.br/noticias/estadao-conteudo/2024/10/17/quintoandardatafolha-65-dos-brasileiros-deixaram-de-negociar-imovel-pelo-preco-diz-estudo.htm>. Acesso em: 6 jun. 2025.
