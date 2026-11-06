---
status: accepted
---

# Perfil público do GitHub via Profile README

Vamos usar um repositório público com o mesmo nome do usuário do GitHub e um `README.md` na raiz como a página inicial do perfil. O conteúdo seguirá o estilo visual Studio: escuro quando o tema do GitHub permitir, compacto, com sensação de estúdio pessoal, status atual, projetos em destaque e uma descrição genérica de trabalhos privados. A grade de contribuições continuará sendo a fonte principal de atividade, com contribuições privadas exibidas somente de forma anonimizada quando essa opção estiver habilitada.

## Contexto

O perfil precisa parecer atual e pessoal, mostrar que existe trabalho em andamento e permitir que visitantes entendam rapidamente a área de atuação. Ao mesmo tempo, alguns projetos não podem ser descritos em detalhe. A solução precisa ser fácil de editar e não deve depender de revelar nomes de clientes, repositórios privados, métricas internas ou arquitetura proprietária.

## Decisão

1. Criar um repositório público chamado exatamente como o nome de usuário do GitHub.
2. Usar o `README.md` desse repositório como página de perfil, com o modelo presente neste projeto.
3. Adotar o estilo Studio: cabeçalho curto, status de trabalho, seções com prefixo `/`, blocos de projetos em tabela e uma paleta escura representada por estrutura, contraste e poucos badges. A cor final pode variar conforme o tema claro/escuro escolhido pelo visitante no GitHub.
4. Descrever projetos privados somente por domínio, tipo de produto ou resultado. Não incluir nomes internos, links, clientes, números ou detalhes técnicos não públicos.
5. Fixar de três a cinco repositórios ou gists públicos que representem melhor o trabalho atual.
6. Tratar badges, cards de estatísticas e animações como opcionais. Só serão usados se melhorarem a leitura e não criarem dependência ou exposição desnecessária.

## Modelos de página para consultar

- [Como criar e gerenciar um Profile README - GitHub Docs](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme)
- [Como o perfil e a grade de contribuições funcionam - GitHub Docs](https://docs.github.com/en/account-and-profile/concepts/contributions-on-your-profile)
- [Como mostrar ou ocultar contribuições privadas - GitHub Docs](https://docs.github.com/en/account-and-profile/how-tos/contribution-settings/manage-visibility-settings-for-private-contributions-and-achievements)
- [Como fixar repositórios e gists - GitHub Docs](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/pinning-items-to-your-profile)
- [Coleção Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [Coleção Creative Profile README](https://github.com/coderjojo/creative-profile-readme)
- [Cards de estatísticas para README - GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Texto animado opcional para README - Readme Typing SVG](https://github.com/DenverCoder1/readme-typing-svg)

O arquivo [`README.md`](../../README.md) deste projeto é o modelo Studio recomendado: moderno, visual e sem dados fictícios sobre a carreira. Basta substituir os campos entre colchetes e remover os comentários HTML.

## Consequências

### Benefícios

- A página fica no próprio GitHub e pode ser editada como código.
- O visitante encontra uma narrativa curta antes da lista de repositórios.
- O estilo Studio cria mais personalidade sem depender de imagens ou serviços externos.
- Projetos privados podem ser contextualizados sem expor informação confidencial.
- O layout é reversível: se a identidade visual mudar, basta editar o README.

### Custos e cuidados

- O perfil exige manutenção ocasional para não ficar desatualizado.
- O GitHub não permite controlar completamente a cor de fundo do README; a sensação Studio vem do layout, contraste, tags e organização, e deve funcionar nos temas claro e escuro.
- Cards e badges de terceiros podem falhar, carregar lentamente ou expor dados agregados; por isso não são obrigatórios.
- A atividade privada não deve ser usada como prova detalhada de um projeto: quando compartilhada no perfil, ela aparece sem os detalhes do repositório.
- O nome do repositório precisa continuar igual ao nome de usuário para o recurso funcionar.

## Critério de atualização

Revisar o README quando houver mudança de foco, novo projeto público relevante ou alteração nos links de contato. Antes de publicar, fazer uma leitura como visitante deslogado e confirmar que nenhuma informação privada aparece por acidente.

## Revisão: vitrine de produto

O perfil agora começa com uma bio curta em inglês de Rafael Bezerra, Backend Developer no Grupo Boticário, seguida por uma vitrine do Cultura em Jeri. O projeto público é descrito pelo que o visitante consegue ver: mapa cultural, eventos e perfis locais. O README aponta para a plataforma, sem vincular o repositório privado nem expor implementação interna.

O cabeçalho usa um SVG local para dar identidade visual ao perfil. A experiência do projeto deve ser mostrada por uma captura ou GIF da interface pública atual assim que houver mídia fiel. A imagem de prévia social atual do site foi descartada porque mostra uma versão antiga. Antes de publicar uma gravação, conferir todos os quadros para evitar nomes, dados pessoais e elementos de sessão privada.
