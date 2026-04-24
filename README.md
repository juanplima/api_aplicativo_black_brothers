# 💪 Black Brothers API

API REST desenvolvida para suportar um aplicativo de gestão de academias, com foco em controle de usuários, treinos, dietas e planos.

O projeto foi construído com uma arquitetura simples e escalável, utilizando Flask, SQLAlchemy, Azure App Service.

---

## 🚀 Visão Geral

Essa API é responsável por centralizar e gerenciar os dados de uma aplicação mobile de academia, permitindo:

- Cadastro e gerenciamento de alunos
- Controle de treinos e dietas
- Gestão de academias e funcionários
- Estrutura de planos e relacionamento com usuários

A aplicação segue o padrão de separação por camadas, facilitando manutenção e evolução.

---

## 🏗️ Arquitetura

O projeto foi estruturado de forma modular:
.
├── app.py # Inicialização da aplicação
├── models.py # Modelos de dados (ORM)
├── routes.py # Endpoints da API
├── extensions.py # Configuração de extensões (DB, etc)


Essa separação permite:
- Reutilização de código
- Facilidade para escalar o projeto
- Melhor organização para times

---

## ⚙️ Tecnologias Utilizadas

- Python
- Flask
- SQLAlchemy
- MySQL
- Azure App Service
- Docker
- dotenv

---

## 🗄️ Modelagem de Dados

A API foi construída com base em entidades principais do domínio de academias:

- **Pessoa**
- **Aluno**
- **Empregado**
- **Academia**
- **Treino**
- **Dieta**
- **Plano**

Os relacionamentos foram modelados utilizando SQLAlchemy ORM, garantindo integridade e flexibilidade.

---

## 🔌 Integração com Banco de Dados

A conexão com o banco é feita via variável de ambiente:

```env
DB_URL=mysql+pymysql://user:password@host/database
Utilizando SQLAlchemy como camada de abstração.
▶️ Como executar o projeto
1. Clonar o repositório
git clone https://github.com/juanplima/api_aplicativo_black_brothers.git
cd api_aplicativo_black_brothers
git clone https://github.com/juanplima/api_aplicativo_black_brothers.git
cd api_aplicativo_black_brothers
2. Criar ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
3. Instalar dependências
pip install -r requirements.txt
pip install -r requirements.txt
4. Configurar variáveis de ambiente

Crie um arquivo .env:
DB_URL=your_database_url
5. Rodar a aplicação
python app.py
📡 Endpoints

A API segue padrão REST e expõe endpoints para operações CRUD das entidades principais.

Exemplos:

GET /alunos
POST /alunos
GET /treinos
POST /dietas

📈 Possíveis Evoluções
Autenticação com JWT
Deploy em nuvem (AWS / GCP)
Containerização com Docker
Documentação com Swagger/OpenAPI
Testes automatizados (Pytest)
Versionamento de API
💡 Sobre o Projeto

Esse projeto foi desenvolvido como parte de um sistema completo de academia, incluindo:

Aplicativo mobile (Flutter)
API backend (este repositório)
Banco de dados relacional

O objetivo foi simular um cenário real de produção, com foco em organização, escalabilidade e boas práticas.

