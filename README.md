https://nimble-nougat-85bfe0.netlify.app
# Trabalho-Franciely
Trabalho da matéria de soft seguro
# 📖 Sobre o projeto

O **Paulo Web Store** é uma livraria online que permite:

- **Visitantes** navegarem pelo catálogo, buscarem e filtrarem livros
- **Clientes** criarem conta, fazerem login, comprarem livros e acompanharem seus pedidos
- **Administradores** gerenciarem o catálogo, os pedidos, os usuários e visualizarem a auditoria do sistema

O grande diferencial é a **separação rígida de papéis** garantida no banco de dados (RLS + triggers + funções `security definer`), de forma que **mesmo que o front-end seja burlado**, o banco bloqueia acessos indevidos.

#  Funcionalidades

# 👤 Visitante
- Ver catálogo de livros (título, autor, preço, estoque)
- Buscar por título, autor ou categoria
- Filtrar por categoria
- Criar conta

- # 🛒 Cliente
- Login e logout
- Adicionar, alterar e remover itens do carrinho
- Finalizar pedido (respeitando o estoque)
- Ver histórico de pedidos com filtro por status
- Ver detalhes de um pedido
- Cancelar pedido com status `Recebido`
- Alterar a própria senha
- Recuperar senha por e-mail

#🛠️ Administrador
- Cadastrar, editar e excluir livros
- Ver todos os pedidos e alterar status
- Cancelar pedido (com devolução de estoque)
- Promover/rebaixar usuários
- Visualizar log de auditoria

# 🧰 Tecnologias utilizadas
| Camada             | Tecnologia |
| **Front-end**      | HTML5, CSS3, JavaScript (ES6+) |
| **Backend**        | Supabase (Auth + PostgREST) |
| **Banco de dados** | PostgreSQL 15 |
| **Autenticação**   | Supabase Auth (bcrypt + JWT) |
| **Segurança**      | Row Level Security (RLS), triggers, funções `security definer` |
| **Hospedagem**     | GitHub Pages, netlify |
