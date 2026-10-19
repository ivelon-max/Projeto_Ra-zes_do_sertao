# Raízes do Sertão — Catálogo Cultural

Site responsivo em HTML, CSS e JavaScript puro. Não precisa instalar dependências para visualizar a interface.

## Como executar

1. Extraia a pasta `catalogo-cultural-sertao`.
2. Abra `index.html` no navegador.

Para um ambiente local mais consistente, execute um servidor estático na pasta, por exemplo:

```bash
python -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Páginas incluídas

- Início
- Catálogo de agentes com busca e filtros
- Perfil individual de agente
- Municípios e página individual por município
- Manifestações culturais e páginas de categoria
- Patrimônio e memória
- Sobre o projeto e formulário de sugestão
- Área administrativa com dashboard
- CRUD de agentes e registros de memória
- Gerenciamento de categorias e municípios
- Lista local de sugestões recebidas

## Área administrativa demonstrativa

- Usuário: `admin`
- Senha: `sertao2026`

**Importante:** esse login é demonstrativo, executado no navegador. Não o utilize para proteger dados em um site público. Para produção, integre autenticação real (por exemplo, Supabase Auth), políticas de acesso no servidor e banco de dados remoto.

## Persistência

Os cadastros são salvos em `localStorage` do navegador. Isso significa que os dados ficam apenas no navegador e dispositivo em que foram cadastrados. Não há sincronização entre pessoas ou dispositivos. O formulário de sugestão também salva localmente.

Para uso público real, conecte a aplicação a um backend e migre os dados para um banco persistente.

## Dados e revisão editorial

Os 15 registros fornecidos foram incluídos como ponto de partida: 14 associados a Monsenhor Tabosa e 1 a Boa Viagem. Dois registros históricos de Monsenhor Tabosa e o registro de Dr. Quiboa aparecem identificados como memória histórica. As biografias e as fontes devem ser confirmadas com os agentes, comunidades e fontes públicas antes de publicação institucional. O campo de verificação do painel serve para controle editorial, não é uma certificação externa.

As imagens dos cartões são avatares tipográficos para evitar retratos inventados. O hero usa uma ilustração vetorial abstrata em CSS.

## Arquivos

- `index.html`: estrutura e navegação principal.
- `styles.css`: design responsivo e componentes visuais.
- `data.js`: registros iniciais e categorias.
- `app.js`: rotas, renderização, filtros, formulários, CRUD e persistência.
- `README.md`: instruções e limitações.

## Limitações conhecidas

Este pacote é um site funcional de demonstração front-end. Antes de disponibilizá-lo na internet:
- substituir login demonstrativo por autenticação real;
- conectar banco de dados e armazenamento de imagens;
- configurar envio centralizado de sugestões;
- revisar fontes e biografias;
- adicionar autorização e políticas de privacidade;
- testar segurança, acessibilidade e desempenho em produção.
