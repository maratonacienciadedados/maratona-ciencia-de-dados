# Projeto Prático

04 a 7 de Abril de 2021 às 20h

# 🤔 Etapa 1 - Entendendo o Problema

---

- Predição de custos de uma campanha de Marketing.

# 🧩 Etapa 2 - Coletando os Dados

---

- Lembra que eu te contei que os dados podem estar em diversas fontes?
- No nosso caso, estamos usando um arquivo xlsx.
    
    [Datasets - Google Drive](https://drive.google.com/drive/folders/1S82BLgDRpEKJHw71gr51Zv4pPAo0RAKq?usp=sharing)
    
- Biblioteca Pandas
    
    [pandas](https://pandas.pydata.org/)
    
    - Métodos importantes 👇
        
        ```python
        #Método utilizado para leitura de arquivos em csv
        df.read_csv()
        ```
        
        ```python
        #Método utilizado para leitura de arquivos em excel
        df.read_excel()
        ```
        

# **📊** Etapa 3 - EDA, Storytelling e Visualização

---

- Na maioria dos casos a gente entra nessa etapa sem saber o que tem nas mãos.
    - Seu trabalho é mergulhar nos dados que coletou visando encontrar padrões, anomalias, testar hipóteses.
        - Dados → Informação → Insights
    - Nossa função e dar sentido aos dados, trazendo contexto, narrativa e insights.
- Biblioteca Pandas
    
    [pandas](https://pandas.pydata.org/)
    
- Métodos Importantes
    
    ```python
    #Retorna as n primeiras linhas do conjunto de dados
    df.head(n=5)
    ```
    
    ```python
    #Resumo do DataFrame
    df.info()
    ```
    
    ```python
    #Número de linhas e colunas do DataFrame
    df.shape
    ```
    
    ```python
    #Renomear Colunas
    df.rename(columns={'NomeAntigo': 'NovoNome'}, inplace = True)
    ```
    
    ```python
    #Estatística Descritiva
    df.describe()
    ```
    
    ```python
    #Retorna quais são os valores únicos (exclusivos)
    df.unique()
    ```
    
    ```python
    #Contagem de valores únicos (exclusivos)
    df.value_counts()
    ```
    
    ```python
    #Identificar dados faltantes
    df.isnull()
    #Dá até pra encadear métodos
    df.isnull().sum()
    df.isnull().sum().sort_values(ascending=False)
    ```
    
    ```python
    #Identificar Outliers
    plt.figure(figsize=(12,6))
    df.boxplot("NomeDaColuna")
    plt.show()
    ```
