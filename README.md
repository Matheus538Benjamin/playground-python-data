# 🔥 Mini Pokédex com Python e PokéAPI

Seja bem-vindo(a) à sua primeira mini Pokédex!  
Aqui, vamos montar um projeto simples em Python que **busca dados reais da internet** sobre três Pokémons famosos: **Charmander**, **Charmeleon** e **Charizard**. Depois, salvamos essas informações em uma tabela organizada, guardamos num banco de dados e até criamos alertas automáticos. 💾⚠️

Ferremantes utilizadas
- APIs (pra buscar dados da internet)
- Pandas (pra criar tabelas e tratar dados)
- SQLite (pra salvar tudo num mini banco)
- Jupyter Notebook (pra rodar e testar o código aos poucos)

---

# 📘 Descrição do Notebook

Este notebook realiza a **extração, tratamento, armazenamento e validação de dados** da **Pokémon API**, com foco nos Pokémons **Charmander**, **Charmeleon** e **Charizard**.

As principais etapas deste processo são:

## 🔹 1. Extração de Dados
- Utilização da biblioteca `requests` para acessar a API pública da PokéAPI;
- Requisição de informações dos Pokémons selecionados por meio de suas URLs individuais.

## 🔹 2. Verificação de Respostas
- Checagem do código de status HTTP (`status_code`);
- Exibição de alertas personalizados caso ocorra falha na obtenção de dados.

## 🔹 3. Criação de Tabelas Individuais (DataFrames)
Para cada Pokémon, são extraídos e organizados os seguintes dados:
- **Nome**
- **Experiência Base**
- **Altura**
- **Peso**
- **ID**

## 🔹 4. Unificação e Tratamento de Dados
- Junção dos DataFrames em uma única tabela;
- Padronização dos nomes das colunas com `str.title()`;
- Preenchimento de valores ausentes com `fillna(0)`;
- Conversão dos tipos de dados para `float` quando necessário;
- Padronização dos nomes dos Pokémons com `str.title()`.

## 🔹 5. Visualização Final
- Exibição da tabela final tratada com `display()` para facilitar a leitura.

## 🔹 6. Armazenamento em Banco de Dados
- Utilização do `sqlite3` para criar e conectar ao banco local `pokemons.db`;
- Salvamento da tabela no banco com o nome `tabela_pokemons`.

## 🔹 7. Validação dos Dados
- Leitura direta dos dados armazenados no banco;
- Exibição da tabela recuperada com `display()`.

## 🔹 8. Sistema de Alerta
- Verificação automática de Pokémons com **experiência base acima de 200**;
- Geração de mensagens de alerta com `print()` para destacar os casos encontrados.

> 💡 Este notebook demonstra, de forma prática, como integrar APIs, tratar dados com `pandas` e armazenar resultados em um banco de dados local com `sqlite3`.

---

## 🧠 Pré-requisitos

Antes de rodar o projeto, você precisa ter:

✅ **Python instalado** no seu computador (versão 3.8 ou superior)  
✅ **Jupyter Notebook** ou **VSCode com extensão Jupyter** instalado  

---

## ⚙️ Passo a passo pra rodar

### 1. Baixe o projeto

Você pode baixar o ZIP direto aqui no GitHub (botão verde “Code > Download ZIP”)  
Ou clonar com Git:

```bash
git clone https://github.com/Matheus538Benjamin/playground-python-data/blob/main/obter_dados_api.ipynb
cd pokedex

## 👩‍💻 Quem fez

Esse projeto foi criado por Matheus Benjamin Aquino Silva. 

- GitHub: [github.com/seu-usuario](https://github.com/Matheus538Benjamin)
