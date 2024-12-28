<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->
B3 Scraping e Evaluation

#### Aluno: [Thiago Correia Umbelino](https://github.com/thiago-umbelino)
#### Orientadora: [Evelyn Batista](https://github.com/evysb).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

<!-- para os links a seguir, caso os arquivos estejam no mesmo repositório que este README, não há necessidade de incluir o link completo: basta incluir o nome do arquivo, com extensão, que o GitHub completa o link corretamente -->
- [Link para o código](https://github.com/link_do_repositorio). <!-- caso não aplicável, remover esta linha -->

---

### Resumo

O Presenta trabalho visa aplicar os conhecimentos adquiridos ao longo do cusro BI Master da PUC-Rio utilizando as técnicas de Web Scraping e modelagem de aprendizado de máquina na intenção de indicar o valor dos papeis de empresas listadas na B3. 

### Abstract

This work aims to apply the knowledge acquired during the BI Master course at PUC-Rio using Web Scraping and machine learning modeling techniques to indicate the value of the securities of companies involved in B3. The Web Scraping technique will be applied to a public website called fundamentus (www.fundamentos.com.br), which compiles information on the fundamentals of companies. After capturing this information, the data will be stored in a database to then be explored and applied to the model to address the value of the securities of this company.

### 1. Introdução

No mundo dos investimentos um dos grandes desafios é julgar o valor de um papel, o chamado evaluation de uma empresa. Existem diversas variáveis que implicam no valor de um papel listada na bolsa, além de todo o contexto de uma economia global, e algumas dessas variáveis são os indicadores funcamentais. Valores de lucro sobre investimento, EBITA, valor 

O Presenta trabalho visa aplicar os conhecimentos adquiridos ao longo do cusro BI Master da PUC-Rio utilizando as técnicas de Web Scraping e modelagem de aprendizado de máquina na intenção de indicar o valor dos papeis de empresas listadas na B3.

A técnica de Web Scraping será aplicada em um site público chamado fundamentus (www.fundamentos.com.br), que compila informações dos funamentos das empresas. Após capturar essas informações os dados serão armazenados em um banco de dados para então serem explorados e aplicados ao modelo na intenção aproximar ao valor do papel dessa empresa.

### 2. Dados

Os dados foram resultado da captura do site públicos Fundamentos utilizando a biblioteca selenium ao longo do curso. Após a captura e armazenamento em banco de dados, eles foram saneados retirando colunas fora de contexto, correções de categorias.
Houve uma exploração visual dos dados na intenção de descobrir algum direcionamento da faixa de preços dos papeis, mas as platagens foram inconclusivas.

### 3. Modelagem

Foram testados 4 modelos de redes neurais na tentativa de encontrar o evaluation sitado anteriormente. Um modelo de regressão sequencial de camandas densas, um segundo modelo utilizando camada convolucional, o terceiro utilizando camadas LSTM e densas e por último um modelo híbrido utilizando camadas Convolucionais e LSTM.   

### 4. Resultados

#### 4.1 Modelo Sequencial Dense

Apresentou uma curva de aprendizado promissora, mas ainda bem distante do valuation real.

#### 4.2 Modelo Convolucional

Obteve o pior desempenho de apresendizado.

#### 4.3 Modelo LSTM Dense

Esse modelo também não apresentou uma boa curva de aprendizado com valores muito distantes do evaluation.

#### 4.4 Modelo Híbrido

Já o modelo híbrido apresentou uma curva de aprendizado interessante, se aproximando do valor do evaluation conforme a época avança, pode apresentar um bom desempenho com um poder computacional maior do que este estudo.

Abaixo a tabela demonstrativa dos resultados.

Alternativa   | MSE | MAE | Tempo 
--- | --- | --- | --- 
4.1:    | 142342.4062 | 20.8610  | 99.2 
4.2:	| 267047425644105139054740242432.0000 | 269140484947968.0000	| 307.7
4.3:	| 697217.4375	| 87.6634	| 3570.7
4.4:	| 503733.3438	| 43.7368	| 940.6

### 4. Conclusões

Infelizmente os resultados do estudo não chegaram a um modelo aplicável para se fazer o evaluation de uma companhia, porém o modelo híbrido se demonstrou promissor e com um poder computacional maior é possível se ter resultados interessantes.

---

Matrícula: 221.100.754

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
