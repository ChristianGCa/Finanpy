# 5. Diretrizes e Convenções

Para garantir a qualidade, consistência e manutenibilidade do código, o projeto Finanpy segue as diretrizes descritas abaixo.

## 5.1 Padrões de Código

- **PEP 8**: Todo o código Python deve seguir rigorosamente as convenções da [PEP 8](https://www.python.org/dev/peps/pep-0008/). Recomenda-se o uso de linters como `flake8` ou `black` para formatação automática.
- **Aspas Simples**: Para strings em Python, utilize aspas simples (`'`) como padrão, a menos que a string contenha uma aspa simples, caso em que aspas duplas (`"`) são permitidas.
- **Linguagem**: Todo o código, incluindo comentários, nomes de variáveis, funções e classes, deve ser escrito em **inglês**.

## 5.2 Estrutura de Apps Django

- **Responsabilidade Única**: Cada app Django deve ter uma responsabilidade clara e bem definida, conforme descrito na seção de arquitetura. Evite acoplar funcionalidades de diferentes domínios no mesmo app.
- **Models**: Todos os models devem incluir campos de data de criação e atualização para facilitar a auditoria.
  ```python
  created_at = models.DateTimeField(auto_now_add=True)
  updated_at = models.DateTimeField(auto_now=True)
  ```

## 5.3 Convenções de Nomenclatura

- **Variáveis e Funções**: Use `snake_case` (ex: `calculate_total`).
- **Classes**: Use `PascalCase` (ex: `TransactionHistory`).
- **Constantes**: Use `UPPERCASE_SNAKE_CASE` (ex: `DEFAULT_CURRENCY`).
- **Templates**: Nomeie os arquivos de template de forma descritiva e utilize uma estrutura de pastas que reflita o app correspondente (ex: `transactions/transaction_list.html`).

## 5.4 Commits

Siga um padrão de commits semânticos para manter o histórico do Git claro e legível. O formato geral é:

`<tipo>(<escopo>): <descrição>`

- **Tipos comuns**:
  - `feat`: Uma nova funcionalidade.
  - `fix`: Uma correção de bug.
  - `docs`: Mudanças apenas na documentação.
  - `style`: Mudanças que não afetam o significado do código (formatação, etc.).
  - `refactor`: Uma refatoração de código que não corrige um bug nem adiciona uma funcionalidade.
  - `test`: Adicionando ou corrigindo testes.
  - `chore`: Mudanças em build, dependências ou ferramentas.

- **Exemplo**:
  ```
  feat(accounts): add feature to create bank accounts
  ```
  ```
  fix(transactions): correct balance calculation after deleting a transaction
  ```
