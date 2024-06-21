# Executando Hybrid_Systems

Este guia fornece instruções sobre como executar o arquivo `Hybrid_Systems.ipynb` no **Google Colab**. O notebook faz o processo de clonar esse repositório do GitHub e realiza operações de push no mesmo do conteúdo processado. Certifique-se de verificar o armazenamento disponível no seu Google Drive e alterar a primeira célula de código preenchendo os campos necessários.

## Requisitos

- Conta no GitHub
- Google Drive com espaço de armazenamento suficiente

## Passos para Execução

### 1. Configurar a Primeira Célula de Código

Antes de executar o notebook, você precisa preencher as seguintes variáveis na primeira célula de código:

- **email_github**: Seu email do GitHub
- **username_github**: Seu nome de usuário do GitHub
- **token**: Seu token de acesso pessoal do GitHub (obtenha-o [aqui](https://github.com/settings/tokens))
- **csv_path**: Caminho para o arquivo CSV que será usado (por padrão, `./data/NH4Complete.csv`)
- **path**: Caminho onde os resultados serão salvos (por padrão, `./Hybrid System/Resultados/NH4Complete`). A última pasta, após Resultados, não precisa ser pré-existente.

```python
# Link para gerar token: https://github.com/settings/tokens
email_github = ""
username_github = ""
token = ""
csv_path = "./data/NH4Complete.csv"
path = './Hybrid System/Resultados/NH4Complete'
```

### 2. Executar o Notebook no Google Colab

1. **Abrir o Google Colab**: Vá para [Google Colab](https://colab.research.google.com/).
2. **Carregar o Notebook**: Carregue o arquivo `Hybrid_Systems.ipynb`.
3. **Montar o Google Drive**: Execute a célula para montar seu Google Drive.
4. **Clonar o Repositório e Configurar Git**: Execute as células para clonar o repositório e configurar as credenciais do Git.
5. **Verificar e Alocar Armazenamento**: Certifique-se de que há espaço suficiente no seu Google Drive.
6. **Alterar Caminhos (se necessário)**: Se estiver usando outro arquivo CSV, altere `csv_path` e `path` de acordo.

### 3. Executar o Código

Após configurar e verificar os pré-requisitos, execute todas as células do notebook para completar o processo.

## Executar o Código para Vários Datasets

Existe uma versão do notebook, `Múltiplas_Tabelas.ipynb` que pode ser utilizada para executar o código em todos os datasets de NH4 que passaram pelo processo de imputação. A configuração inicial é semelhante, com algumas alterações adicionais.

### Configurar a Primeira Célula de Código

Preencha as seguintes variáveis na primeira célula de código:

- **email_github**: Seu email do GitHub
- **username_github**: Seu nome de usuário do GitHub
- **token**: Seu token de acesso pessoal do GitHub (obtenha-o [aqui](https://github.com/settings/tokens))

### Definir um Subconjunto de Tabelas

Na primeira célula da seção "Execução", você pode definir um subconjunto das tabelas que deseja usar, alterando a variável `csv_files`.

```python
# Link para gerar token: https://github.com/settings/tokens
email_github = ""
username_github = ""
token = ""
# Para definir um subconjunto das tabelas que deseja usar, redefina a variável csv_files
# Exemplo para usar um subconjunto:
# csv_files = csv_files[28:29]
```

### Passos para Execução em Modo Batch

1. **Abrir o Google Colab**: Vá para [Google Colab](https://colab.research.google.com/).
2. **Carregar o Notebook**: Carregue o arquivo com a versão em batch do código.
3. **Montar o Google Drive**: Execute a célula para montar seu Google Drive.
4. **Clonar o Repositório e Configurar Git**: Execute as células para clonar o repositório e configurar as credenciais do Git.
5. **Verificar e Alocar Armazenamento**: Certifique-se de que há espaço suficiente no seu Google Drive.
6. **Alterar Caminhos e Definir Subconjunto (se necessário)**: Se estiver usando outro arquivo CSV, altere `csv_path`, `path` e a variável `csv_files` de acordo.

### Executar o Código

Após configurar e verificar os pré-requisitos, execute todas as células do notebook para completar o processo.

## Observações Finais

- **Armazenamento no Google Drive**: Verifique sempre o armazenamento disponível no Google Drive antes de executar os notebooks, pois as operações podem consumir bastante espaço.
- **Tokens do GitHub**: Mantenha seus tokens de acesso pessoal seguros e não os compartilhe publicamente.

Seguindo essas instruções, você deve ser capaz de executar o arquivo `Hybrid_Systems.ipynb` no Google Colab com sucesso, bem como a versão para vários datasets.