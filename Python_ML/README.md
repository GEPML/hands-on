# Hands-on: Python e ML com Random Forest

Prática (hands-on) de Python com aprendizado de máquina (*Machine Learning*) com Random Forest. O objetivo principal é adicionar um novo recurso (*feature*) na implementação de um Random Forest modificado: `random-forest-mc`. Esse recurso é para predizer valores faltantes utilizando as árvores de decisão.

## Cronograma

O dia 1 serve para quem usa Windows e precisa de ajuda para configurar um ambiente basedo em container, assim pode-se obter um mesmo ambiente que seja invariante ao computador do usuário. Para usuários Linux, o dia 1 pode ser ignorado. O dia 2 serve de base para o dia 3, sendo o dia 1 opcional.

São previstas no total 3 encontros de 2 horas e 30 min cada, com intervalo de 30 minnutos.

### Dia 1:

1. Usar a aplicação `random-forest-mc`.  
1.1. Configurar o Docker Desktop no Windows.  
1.2. Baixar o repositório, instalar e usar a aplicação.  
1.3. Rodar os testes unitários.  

### Dia 2:

2. Entender a aplicação.  
2.1. Random Forest.  
2.2. Monte Carlo.  
2.3. Otimização indireta usando Monte Carlo.  

Material de apoio:   
    - [O que é a simulação de Monte Carlo?](https://aws.amazon.com/pt/what-is/monte-carlo-simulation/)  
    - [Wikipédia: Monte Carlo method.](https://en.wikipedia.org/wiki/Monte_Carlo_method)  
    - Exemplos com Python: [cálculo integral](https://github.com/ysraell/examples/tree/master/Monte_Carlo) e [cálculo do $\pi$](https://github.com/ysraell/examples/blob/master/Classical_Problems_CS_wPython/1.4.ipynb).  
    - [Understand Random Forest Algorithms With Examples (Updated 2023).](https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/)  
    - [The Basics of Decision Trees.](https://medium.datadriveninvestor.com/the-basics-of-decision-trees-e5837cc2aba7)  
    - [Laboratory of Decision Tree and Random Forest.](https://github.com/ysraell/random-forest-lab)  

### Dia 3:

3. Desenhar a nova *feature*: 
- **Entrada:** um `dataframe` com 1 ou mais linhas, contendo valores faltantes e uma lista de possíveis valores para cada coluna que contém valores faltantes. O `dataframe` pode ou não conter as classes.
- **Saída:** um `dataframe` contendo as linhas do de entrada com todas as possíveis variações e as probabilidades. Caso as classes não sejam dadas, inclui as variações para cada classe.  
3.1. PoC: desenvolver a *feature* em um notebook Jupyter.  
3.2. Implementar na biblioteca.  
3.3. Escrever os testes unitários e garantir a cobertura de código.  
4. Publicar a nova versão.  
4.1. PR -> `main` *branch*.  
4.2. Publicar no PyPI.  
4.3. Validar o pacote num ambiente isolado.  

