# INTELIGÊNCIA URBANA E MOBILIDADE: ANÁLISE SISTÊMICA DE FLUXOS E RESILIÊNCIA EM REDES DE TRANSPORTE PÚBLICO ATRAVÉS DA CIÊNCIA DE DADOS E TEORIA DOS GRAFOS

O tema proposto mergulha no conceito de "Smart Cities" (Cidades Inteligentes), aplicando Ciência de Dados para resolver um dos maiores problemas das metrópoles paulistas: a mobilidade urbana. O transporte público gera uma quantidade colossal de rastros digitais, desde dados de GPS dos ônibus até os registros de bilhetagem eletrônica. Analisar esses dados permite **identificar gargalos, propor novas rotas e otimizar a frequência das linhas**.


## Contexto Urbano e a Teoria dos Grafos
A mobilidade urbana pode ser modelada através da Teoria dos Grafos, onde as paradas de ônibus e estações de metrô são "nós" e as rotas são "arestas". A aplicação de algoritmos de centralidade permite identificar quais pontos do sistema são críticos para a resiliência da rede. Se um nó com alta centralidade de intermediação sofre uma interrupção, o impacto se propaga por todo o sistema, causando atrasos em cascata.

O uso de dados abertos, como os fornecidos pela SPTrans no sistema GTFS (*General Transit Feed Specification*), permite a construção de simulações de fluxo. Além disso, a integração com dados de sensores de tráfego e até dados de redes sociais (para identificar eventos que alteram a demanda) oferece uma visão holística da dinâmica da cidade.

## Clustering e Segmentação de Padrões de Deslocamento
Uma abordagem poderosa neste tema é o uso de algoritmos de agrupamento (Clustering), como o K-Means ou o DBSCAN, para identificar padrões de deslocamento da população. Ao agrupar usuários que realizam trajetos semelhantes em horários parecidos, a gestão pública pode planejar serviços de transporte sob demanda ou ajustar a frota de maneira dinâmica.

O desafio técnico reside no processamento de grandes volumes de dados geoespaciais. O uso de bibliotecas como Geopandas e PySAL em Python é indispensável para realizar operações espaciais, como o "spatial join" e o cálculo de distâncias em grandes matrizes. A visualização de dados espaciais através de mapas de calor (Heatmaps) e mapas de fluxo é crucial para que o TCC tenha uma camada de comunicação visual eficaz, facilitando a interpretação por gestores públicos.

## Avaliação de Impacto e Sustentabilidade
Além da otimização do tempo, a Ciência de Dados pode ser usada para medir o impacto ambiental do transporte. Através de modelos que estimam a emissão de CO2 com base no tempo de permanência dos veículos em congestionamentos e no tipo de combustível, o TCC pode propor estratégias para uma mobilidade mais verde. Esta dimensão de sustentabilidade alinha o trabalho com as agendas globais de desenvolvimento sustentável, elevando seu valor acadêmico e social.

|   |   |   |
|---|---|---|
|**Métrica de Mobilidade**|**Definição**|**Aplicação no TCC**|
|Travel Time Reliability|Variabilidade no tempo de viagem entre dois pontos.|Identificar linhas que precisam de faixas exclusivas.|
|Load Factor|Proporção entre passageiros transportados e capacidade.|Otimizar a frequência de ônibus para evitar superlotação.|
|Connectivity Index|Medida de quão bem conectada está uma região à rede.|Avaliar a equidade no acesso ao transporte em periferias.|
|Deadhead Miles|Distância percorrida por veículos sem passageiros.|Reduzir custos operacionais das empresas concessionárias.|

A aplicação destas métricas, conforme demonstrado na tabela, permite uma análise quantitativa rigorosa do sistema de transporte, fornecendo subsídios para intervenções urbanas baseadas em evidências.