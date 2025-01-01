
### Tendências no Setor Agrícola | Análise de dados com Python

### Objetivo

Commodities são bens de consumo básicos, geralmente matérias-primas, que são produzidos em grande escala e possuem pouca ou nenhuma diferenciação entre os produtores. Exemplos incluem petróleo, ouro, café, soja, trigo, gás natural e minério de ferro.

À vista disso, as informações das matérias-primas são de interesse de toda a população global e o intuito desse Case é encontrar padrões e tendências nas séries históricas das matérias-primas, aplicando técnicas de análises estatísticas. Como as informações das commodities são públicas, são de simples acesso com os dados fornecidos pelo Governo Federal.

### Organização do Projeto

```
├── .gitignore    <- Arquivos e diretórios a serem ignorados pelo Git  
├── LICENSE       <- Licença de código aberto (MIT)  
├── README.md     <- README principal para desenvolvedores que utilizam este projeto  
├── notebooks     <- Cadernos Jupyter contendo análises e experimentos chamado
        ├── Materiais_de_agricultura.ipynb

├── dados         <- Fonte de dados usados no projeto
        ├── agricultural_raw_material.csv

├── images        <- imagens usadas no README.
```

### Detalhes do dataset utilizado

A base de dados contém informações das commodities na granulalidade a nível de mês. Os dados disponíveis são o valor das matérias-primas e o percentual de mudanças dos preços. A consulta fornecida, apresentava muitas informações vazias que passaram por um tratamento prévio para não interferirem nas métricas estatísticas.
 Após o ETL, algumas informações foram desconsideradas conforme a análise preditiva, foram usados somente os dados válidos. 

### Metodologia e Resumo dos Resultados

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

### Ferramentas

 - As ferramentas de visualização: Matplotlib e Seaborn.
 - Construção e Cálculos: Pandas e Numpy.

### Como Reproduzir o Projeto

 - Baixar o arquivo ipynb no repositório.
 - Baixar a fonte de dados na pasta Dados.
   
