# 4. Design System

O design do Finanpy foi construído para ser moderno, limpo e funcional, com foco em um tema escuro que utiliza gradientes e uma paleta de cores harmônica.

## 4.1 Paleta de Cores

#### Cores Primárias
- **Gradiente Principal**: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`
- **Primária**: `#667eea`
- **Acentuação**: `#764ba2`

#### Cores de Fundo (Tema Escuro)
- **Fundo Principal**: `#0f172a`
- **Fundo de Cards**: `#1e293b`
- **Fundo de Hover**: `#334155`

#### Cores de Texto
- **Texto Principal**: `#f1f5f9`
- **Texto Secundário**: `#cbd5e1`
- **Texto Mudo**: `#64748b`

#### Cores de Estado
- **Sucesso (Entradas)**: `#10b981`
- **Erro (Saídas)**: `#ef4444`
- **Aviso**: `#f59e0b`
- **Informação**: `#3b82f6`

## 4.2 Tipografia

- **Fonte Principal**: `Inter`, `system-ui`, `-apple-system`, `sans-serif`
- **Tamanhos Base**:
  - `text-sm`: 14px
  - `text-base`: 16px
  - `text-lg`: 18px
- **Pesos**: `font-normal` (400), `font-medium` (500), `font-semibold` (600), `font-bold` (700)

## 4.3 Componentes

Os componentes são construídos com **TailwindCSS** para garantir consistência e agilidade.

#### Botões
- **Primário**: Fundo em gradiente, texto branco, cantos arredondados (`rounded-lg`).
- **Secundário**: Fundo `bg-secondary`, texto `text-primary`, com borda e transição em hover.

#### Forms
- **Inputs**: Fundo `bg-secondary`, borda `bg-tertiary` e foco com anel `ring-primary-500`.
- **Labels**: Texto `text-secondary` e `font-medium`.

#### Cards
- **Padrão**: Fundo `bg-secondary`, cantos arredondados (`rounded-xl`), sombra (`shadow-lg`) e borda `bg-tertiary`.
- **Destaque**: Fundo em gradiente para informações importantes como saldo total.
