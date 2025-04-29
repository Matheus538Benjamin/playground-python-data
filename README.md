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
Agora também integra as **habilidades** de cada Pokémon e usa um sistema de alerta avançado, inspirado no modelo da Aula 20.

As principais etapas do processo são:

## 🔹 Primeiro passo: Mensagem de Alerta
- Implementação da função `alerta()` para exibir mensagens personalizadas em caso de erro ou eventos específicos.

## 🔹 Etapa 1: Extração dos Dados
- Acesso à PokéAPI usando a biblioteca `requests`;
- Coleta dos dados básicos dos Pokémons: Nome, Experiência Base, Altura, Peso e ID.

## 🔹 Etapa 2: Coleta e Organização
- Coleta adicional das **habilidades** de cada Pokémon;
- Organização dos dados principais + habilidades em um `DataFrame`.

## 🔹 Etapa 3: Tratamento dos Dados
- Padronização dos nomes das colunas usando `str.title()`;
- Preenchimento de valores nulos com `fillna(0)`;
- Conversão dos tipos (`Altura` e `Peso`) para `float`;
- Ajuste de texto para deixar os nomes dos Pokémons formatados.

## 🔹 Etapa 4: Armazenamento no SQLite
- Criação de um banco local `pokemons_v4.db` com `sqlite3`;
- Salvamento dos dados tratados na tabela `tabela_pokemons`.

## 🔹 Etapa 5: Validação
- Leitura dos dados salvos no banco;
- Exibição do conteúdo da tabela para conferir se os dados foram armazenados corretamente.

## 🔹 Etapa 6: Sistema de Alerta
- Verificação automática de Pokémons com **experiência base acima de 200**;
- Emissão de alertas formatados informando nome e experiência do Pokémon.

> 💡 Este notebook é um ótimo exemplo de como integrar APIs, tratar dados com `pandas`, salvar resultados com `sqlite3` e automatizar alertas de validação.

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