# 📊 Sistema de Gerenciamento de Preços Corporativo

Sistema web completo para gestão de tabelas de preços com múltiplos níveis de acesso, importação/exportação de dados, CRUD de produtos e visualização responsiva (tabela ou cards).

![Tela de Login](https://via.placeholder.com/800x400?text=Tela+de+Login+do+Sistema)

---

## 🚀 Funcionalidades

- **Autenticação de usuários** com 4 perfis de acesso distintos.
- **Controle de permissões** conforme o perfil:
  - **Admin:** acesso total (criar, editar, excluir, importar, exportar, ver todas as 8 tabelas de preços).
  - **Gerente:** edita produtos e vê todas as tabelas, mas **não pode importar** dados.
  - **Vendedor:** somente leitura das **Tabelas 1 a 4**.
  - **Representante:** somente leitura das **Tabelas 5 a 8**.
- **CRUD completo** de produtos (criação via importação, edição, exclusão, ativação/desativação).
- **Importação de dados** em dois formatos:
  - Upload de arquivo Excel (.xls, .xlsx)
  - Colagem de texto CSV (separador `;`)
- **Exportação** para CSV e Excel (HTML com extensão .xls).
- **Pesquisa** por código ou descrição (case‑insensitive).
- **Ordenação** dinâmica clicando nos cabeçalhos da tabela.
- **Paginação** configurável (5, 10, 20 ou 50 itens por página).
- **Visualização alternativa** em **Cards** (ideal para dispositivos móveis).
- **Persistência local** – os dados ficam salvos no `localStorage` do navegador (não desaparecem ao recarregar a página).
- **Design responsivo** – adapta-se a diferentes tamanhos de tela.
- **Modal de edição** com validação de preços (não negativos).

---

## 🧪 Credenciais de Teste

| Perfil        | Usuário       | Senha          | Permissões                                 |
|---------------|---------------|----------------|---------------------------------------------|
| Admin         | `admin`       | `admin123`     | Total (edita, importa, exporta)             |
| Gerente       | `gerente`     | `gerente123`   | Edita, vê todas as tabelas, sem importador  |
| Vendedor      | `vendedor`    | `vendedor123`  | Somente leitura – Tabelas 1 a 4             |
| Representante | `representante` | `rep123`     | Somente leitura – Tabelas 5 a 8             |

> ⚠️ As credenciais estão fixas no código – para uso real, devem ser substituídas por autenticação no backend.

---

## 📁 Estrutura do Projeto

O projeto é **monolítico** (um único arquivo HTML), contendo:
