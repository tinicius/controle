## Descrição do Projeto

Este projeto tem como objetivo analisar o Índice de Vegetação por Diferença Normalizada (NDVI) utilizando a teoria de controle. O NDVI é amplamente utilizado no sensoriamento remoto para monitorar a saúde da vegetação. A análise foi realizada para a cidade de Divinópolis-MG, Brasil, utilizando dados do sensor MODIS da NASA.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

- `bra-ndvi-adm2-5ytd.csv`: Arquivo CSV contendo os dados de NDVI para diferentes regiões do Brasil.
- `Trabalho_Controle.ipynb`: Notebook Jupyter contendo a implementação do código para análise e visualização dos dados de NDVI.
- `README.md`: Este arquivo, contendo a descrição do projeto e instruções de uso.

## Implementação

A implementação foi realizada em Python, utilizando bibliotecas como `pandas` para manipulação de dados, `matplotlib` para visualização e `scipy` para ajuste de curvas. A seguir, são descritas as principais etapas da implementação:

1. **Instalação de Dependências**:
    - As bibliotecas necessárias foram instaladas utilizando `pip`.

2. **Leitura e Filtragem dos Dados**:
    - Os dados foram lidos a partir do arquivo CSV `bra-ndvi-adm2-5ytd.csv`.
    - Foi realizado um filtro para selecionar apenas os dados referentes à cidade de Divinópolis-MG.

3. **Análise Temporal do NDVI**:
    - Os dados foram agrupados por mês e ano para calcular a média mensal do NDVI.
    - Foram gerados gráficos para visualizar a variação do NDVI ao longo do tempo.

4. **Ajuste de Curva Senoidal**:
    - Foi utilizado o método de ajuste de curva da biblioteca `scipy` para ajustar uma função senoidal aos dados de NDVI.
    - O ajuste foi visualizado em um gráfico comparando os dados originais com a curva ajustada.

5. **Comparação com Dados Climáticos**:
    - Dados de precipitação e temperatura foram lidos a partir de outro arquivo CSV.
    - Foi gerado um gráfico comparando a precipitação, temperatura e NDVI ao longo do ano de 2024.

## Como Executar

1. Clone o repositório para sua máquina local.
2. Instale as dependências necessárias:
    ```bash
    pip install [nome da biblioteca]
    ```    
4. Abra o notebook `Trabalho_Controle.ipynb` em um ambiente Jupyter e execute as células para reproduzir a análise.


## Referências

- [MODIS NDVI Data](https://modis.gsfc.nasa.gov/data/)
- [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [Scipy Documentation](https://docs.scipy.org/doc/scipy/)
