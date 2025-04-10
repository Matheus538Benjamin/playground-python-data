# 🔥 Mini Pokédex com Python e PokéAPI

Seja bem-vindo(a) à sua primeira mini Pokédex!  
Aqui, vamos montar um projeto simples em Python que **busca dados reais da internet** sobre três Pokémons famosos: **Charmander**, **Charmeleon** e **Charizard**. Depois, salvamos essas informações em uma tabela organizada, armazenamos num banco de dados e até criamos alertas automáticos. 💾⚠️

### 🛠️ Ferramentas utilizadas:
- `requests` (pra buscar dados da internet via API)
- `pandas` (pra criar e tratar tabelas)
- `sqlite3` (pra salvar tudo num mini banco local)
- `Jupyter Notebook` (pra rodar e testar o código passo a passo)

---

# 📘 Descrição do Notebook

Este notebook realiza a **extração, tratamento, armazenamento e validação de dados** da **Pokémon API**, com foco nos Pokémons **Charmander**, **Charmeleon** e **Charizard**.

As principais etapas do processo são:

## 🔹 1. Extração de Dados
- Acesso à PokéAPI com a biblioteca `requests`;
- Coleta dos dados de cada Pokémon por suas URLs específicas.

## 🔹 2. Verificação de Respostas
- Checagem do `status_code` da resposta da API;
- Mensagens de erro personalizadas em caso de falha na requisição.

## 🔹 3. Criação de Tabelas Individuais (DataFrames)
Para cada Pokémon, são organizadas informações como:
- **Nome**
- **Experiência Base**
- **Altura**
- **Peso**
- **ID**

## 🔹 4. Unificação e Tratamento de Dados
- Junção dos DataFrames em uma única tabela;
- Padronização dos nomes das colunas com `str.title()`;
- Preenchimento de valores ausentes com `fillna(0)`;
- Conversão de tipos para `float`, quando necessário;
- Padronização dos nomes dos Pokémons com `str.title()`.

## 🔹 5. Visualização Final
- Exibição da tabela final tratada com `display()` para facilitar a leitura.

## 🔹 6. Armazenamento em Banco de Dados
- Criação de um banco local `pokemons.db` com `sqlite3`;
- Armazenamento da tabela no banco com o nome `tabela_pokemons`.

## 🔹 7. Validação dos Dados
- Leitura direta do banco para conferir os dados salvos;
- Exibição da tabela recuperada com `display()`.

## 🔹 8. Sistema de Alerta
- Checagem automática de Pokémons com **experiência base acima de 200**;
- Geração de alertas com `print()` para destaque.

> 💡 Este notebook é um ótimo exemplo de como integrar APIs, tratar dados com `pandas` e salvar os resultados com `sqlite3`.

---

## 🧠 Pré-requisitos

Antes de rodar o projeto, você precisa ter:

✅ **Python 3.8+ instalado** no seu computador  
✅ **Jupyter Notebook** (ou **VSCode com a extensão Jupyter**)

---

## ⚙️ Como rodar o projeto

### 1. Clone este repositório

Você pode baixar o ZIP direto no botão verde “Code > Download ZIP”  
Ou usar Git:

```bash
git clone https://github.com/Matheus538Benjamin/playground-python-data.git
cd playground-python-data
```

### 2. Rode o notebook

Abra o **Jupyter Notebook** e execute o arquivo `obter_dados_api.ipynb` célula por célula.  
Você verá os dados sendo carregados, tratados e salvos automaticamente.

---

## 👤 Autor

**Matheus Benjamin Aquino Silva**  
🔗 [github.com/Matheus538Benjamin](https://github.com/Matheus538Benjamin)