
### Identificadores de Tendências no Setor Agrícola | Análise de dados 

### Objetivo

Commodities são bens de consumo básicos, geralmente matérias-primas, que são produzidos em grande escala e possuem pouca ou nenhuma diferenciação entre os produtores. Exemplos incluem petróleo, ouro, café, soja, trigo, gás natural e minério de ferro.

À vista disso, as informações das matérias-primas são de interesse de toda a população global e o intuito desse Case é encontrar padrões e tendências nas séries históricas das matérias-primas, aplicando técnicas de análises estatísticas. Como as informações das commodities são públicas, são de simples acesso com os dados fornecidos pelo Governo Federal.

### Detalhes do dataset utilizado

A base de dados contém informações das commodities na granulalidade a nível de mês. Os dados disponíveis são o valor das matérias-primas e o percentual de mudanças dos preços. A consulta fornecida, apresentava muitas informações vazias que passaram por um tratamento prévio para não interferirem nas métricas estatísticas.
 
![image](https://github.com/user-attachments/assets/a751df36-d04a-41a8-a51d-771165946678)

Após o ETL, alguns informações foram desconsideradas conforme foi feito o alinhamento do desenvolvimento, o que foi posto como principal foram os dados válidos. 

![image](https://github.com/user-attachments/assets/1973726c-39f5-4def-b5db-681201d194af)

### Resumo dos Resultados

Uma das principais vantagens das análises estatísticas é a diversidade e a ampla gama de possibilidades que elas oferecem, aliadas a um alto grau de precisão e confiabilidade. Com base nessas características, o indicador escolhido foi a correlação, que mede a relação entre duas variáveis quantitativas contínuas.

A variação percentual das commodities foram usadas.

![gráfico corr %](https://github.com/user-attachments/assets/9a09838c-711e-453b-a93e-23c631979d36)

A partir desses resultados podemos dizer que quase não há relação entre a variação percentual dos preços das matérias-primas

- o valor negativo implica que duas variáveis ​​estão negativamente correlacionadas (um aumento, outro decréscimo)
- Zero implica nenhuma relação, caso contrário, maior o valor maior a chance de relação, preços e seus gráficos de % de mudança

Outra métrica de suma importância é o comparativo entres preços das commodities ao longo do tempo. 

![image](https://github.com/user-attachments/assets/e49ed5aa-2730-49e5-b252-6e2624141693)

Assim como a métrica da variação dos preços.

![image](https://github.com/user-attachments/assets/6a1cea14-cdad-4eb0-9a9c-40a75cc5678d)

Podemos ver o maior percentual de mudança em mais de 60% para madeira serrada macia e o menor percentual de mudança é para madeira compensada em menos de 20%.

Há outras análises no projeto, que retratam comparativos mais interessantes com um nível de detalhamento maior. 
Ademais, um dos pilares da estatística é a análise descritiva que trás a distribuição dos dados em quartis, sendo o principal a mediana, também apresentando na visualização, mas também outros outliers que serão analizados em atualizações futuras no desenvolvimento. Portanto, destaquei indicadores-chave que são cruciais para a tomada de decisões estratégicas, utilizando métodos estatísticos robustos para validar minhas descobertas.

### Ferramentas e Metodologia
 - Python
 - As ferramentas de visualização como Matplotlib e Seaborn foram essenciais para criar gráficos claros e informativos que destacaram as relações entre os diferentes indicadores.
 - A capacidade de Pandas para manipulação eficiente de dados e a flexibilidade do NumPy para cálculos complexos foram fundamentais para o sucesso do projeto.

### Como Reproduzir o Projeto
 - Baixar o arquivo ipynb no repositório.




 
