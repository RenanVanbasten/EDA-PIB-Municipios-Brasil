# Análise Exploratória do Produto Interno Bruto (PIB) dos 100 Maiores Municípios do Brasil

## Introdução
Este relatório apresenta os principais insights obtidos a partir da análise exploratória dos dados do Produto Interno Bruto (PIB) dos 100 maiores municípios do Brasil. O objetivo foi compreender a distribuição geográfica e a concentração econômica do PIB no cenário nacional, identificando padrões e particularidades.

---

## Preparação e Tratamento dos Dados
Os dados brutos continham informações sobre "Municípios e respectivas Unidades da Federação", além de dados do PIB em formato de texto. Para a análise, foram realizadas as seguintes transformações:
* **Extração de Cidades e Estados:** A coluna original de localização foi dividida para criar colunas separadas para `Cidades` e `Estados`.
* **Criação de Regiões:** Uma nova coluna `Regioes` foi criada para agrupar os estados em suas respectivas regiões geográficas (Norte, Nordeste, Centro-Oeste, Sudeste, Sul).
* **Conversão de Tipos:** A coluna de `Produto Interno Bruto a preços correntes (1 000 R$)` foi convertida para um tipo numérico para permitir cálculos e agregações.
* **Limpeza de Posição:** A coluna `Posição ocupada pelos 100 maiores municípios` foi tratada e convertida para um formato numérico para facilitar o ordenamento e a identificação do ranking.

---

## Insights Principais

A análise revelou padrões interessantes sobre a distribuição do PIB e a presença de municípios nos maiores centros econômicos do país.

### 1. Representatividade Regional no Top 100 PIB

A distribuição dos 100 maiores municípios em termos de PIB por região do Brasil demonstra uma clara concentração em algumas áreas:
* **Sudeste:** 55 municípios
* **Sul:** 17 municípios
* **Nordeste:** 14 municípios
* **Centro-Oeste:** 8 municípios
* **Norte:** 3 municípios

É notável a **predominância da Região Sudeste**, abrigando mais da metade dos municípios com os maiores PIBs do país.

### 2. Representatividade Estadual no Top 100 PIB

Aprofundando a análise por estado, a concentração se mantém evidente:
* **São Paulo (SP):** 35 municípios
* **Rio de Janeiro (RJ):** 10 municípios
* **Paraná (PR):** 9 municípios
* **Minas Gerais (MG):** 7 municípios
* **Santa Catarina (SC):** 5 municípios
* **Bahia (BA):** 4 municípios
* **Pará (PA):** 4 municípios
* **Goiás (GO):** 4 municípios
* **Pernambuco (PE):** 3 municípios
* **Rio Grande do Sul (RS):** 3 municípios
* **Espírito Santo (ES):** 3 municípios
* **Mato Grosso (MT):** 2 municípios
* **Distrito Federal (DF):** 1 município
* **Amazonas (AM):** 1 município
* **Ceará (CE):** 1 município
* **Mato Grosso do Sul (MS):** 1 município
* **Maranhão (MA):** 1 município
* **Alagoas (AL):** 1 município
* **Rio Grande do Norte (RN):** 1 município
* **Piauí (PI):** 1 município
* **Paraíba (PB):** 1 município
* **Rondônia (RO):** 1 município
* **Sergipe (SE):** 1 município

### 3. Estados Sem Municípios no Top 100 PIB

Uma observação crucial é que nem todos os estados brasileiros possuem municípios entre os 100 com maior PIB. Os seguintes estados **não têm nenhuma representação** nesta lista:
* **Acre (AC)**
* **Amapá (AP)**
* **Roraima (RR)**
* **Tocantins (TO)**

Essa ausência destaca a concentração econômica em outras regiões e a disparidade regional no desenvolvimento econômico dos maiores centros urbanos.

### 4. Contribuição de Cada Estado para o PIB de Sua Região

A análise da contribuição percentual do PIB de cada estado para o total de sua respectiva região (considerando apenas os municípios no Top 100) revela os "motores" econômicos internos de cada região:

* **Centro-Oeste:**
    * DF: 61.92%
    * GO: 21.89%
    * MS: 7.02%
    * MT: 9.17%
    
    *(Nota: Brasília, no DF, é um caso especial de capital-município-estado.)*

* **Nordeste:**
    * BA: 28.53%
    * PE: 19.72%
    * CE: 16.64%
    * MA: 8.45%
    * AL: 5.84%
    * RN: 5.80%
    * PI: 5.51%
    * PB: 5.30%
    * SE: 4.20%

* **Norte:**
    * PA: 48.40%
    * AM: 42.58%
    * RO: 9.02%

* **Sudeste:**
    * SP: 65.77%
    * RJ: 22.29%
    * MG: 9.42%
    * ES: 2.51%

* **Sul:**
    * PR: 49.17%
    * SC: 25.42%
    * RS: 25.41%

Essa granularidade mostra que, mesmo dentro das regiões, o PIB dos maiores municípios pode ser fortemente concentrado em um ou dois estados.

### 5. Capitais vs. Outros Municípios no Topo do PIB Estadual

Um insight interessante é a identificação de estados onde a capital não é o município com maior PIB (dentro do ranking dos 100 maiores). Isso sugere a presença de outros grandes polos econômicos fora das capitais.
* **Pará (PA):** O município com maior PIB é **Parauapebas** e não a capital (Belém).
* **Santa Catarina (SC):** O município com maior PIB é **Joinville** e não a capital (Florianópolis).

---

## Conclusões e Próximos Passos
A Análise Exploratória de Dados revela uma forte concentração do PIB do Brasil nos municípios da Região Sudeste, com São Paulo e Rio de Janeiro como grandes destaques. A ausência de alguns estados na lista dos 100 maiores PIBs aponta para desigualdades regionais significativas. A contribuição detalhada por estado e a identificação de não-capitais com o maior PIB em seus estados fornecem uma visão mais granular das dinâmicas econômicas.

**Próximos Passos:**
* **Visualização Aprofundada:** Gerar gráficos adicionais (como gráficos para a participação regional no total dos 100, ou um mapa coroplético da distribuição dos municípios no Brasil) para comunicar esses insights de forma ainda mais eficaz.
* **Fatores Explicativos:** Se possível, integrar outros datasets (população, setor econômico dominante) para entender os fatores por trás do alto PIB desses municípios.