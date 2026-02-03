# 2. Arquitetura

## 2.1 Stack Tecnológica

#### Backend
- **Linguagem**: Python 3.13+
- **Framework**: Django 5+
- **Banco de Dados**: SQLite3 (padrão Django)
- **Autenticação**: Django Auth (nativo)

#### Frontend
- **Template Engine**: Django Template Language
- **CSS Framework**: TailwindCSS
- **JavaScript**: Vanilla JS (mínimo necessário)

#### Infraestrutura
- **Ambiente Virtual**: venv
- **Gerenciador de Pacotes**: pip

## 2.2 Estrutura de Apps Django

A estrutura do projeto é organizada em apps com responsabilidades claras:

```
finanpy/
├── core/           # Configurações globais e URLs principais
├── users/          # Extensão do User model do Django
├── profiles/       # Perfis de usuários
├── accounts/       # Contas bancárias
├── categories/     # Categorias de transações
├── transactions/   # Transações financeiras
└── static/         # Arquivos estáticos (CSS, JS, imagens)
```

## 2.3 Requisitos Funcionais

O sistema cobre as seguintes funcionalidades:

- **Autenticação**: Cadastro, login e logout de usuários.
- **Gestão de Perfis**: Visualização e edição de perfis.
- **Gestão de Contas**: CRUD de contas bancárias.
- **Gestão de Categorias**: CRUD de categorias de transações.
- **Gestão de Transações**: CRUD de transações de entrada e saída, com filtros.
- **Dashboard**: Visualização consolidada da situação financeira.
- **Site Público**: Página de apresentação para não autenticados.

## 2.4 Requisitos Não-Funcionais

- **Performance**: Páginas devem carregar em menos de 2 segundos.
- **Segurança**: Senhas com hash, rotas protegidas e isolamento de dados de usuários.
- **Usabilidade**: Interface responsiva, acessível e com mensagens claras.
- **Manutenibilidade**: Código em inglês, seguindo PEP 8 e com responsabilidades bem definidas.
