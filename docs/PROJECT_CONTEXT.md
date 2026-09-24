# Contexto do projeto

Este repositório contém a Home da disciplina Design do portfólio de Arthur. Ela é a primeira parte de um produto maior, que futuramente terá Home raiz e rotas independentes para Design, Vídeo, Game Dev, Mentoria, Sobre, Contato e Links.

## Estado atual

- A base visual é a Pictorial V08, refinada aqui como V09.
- O conteúdo e vários projetos ainda são placeholders.
- O site é estático e publicado por GitHub Pages.
- `index.html` ainda concentra estrutura, estilos e interações para evitar uma migração prematura durante a fase de direção visual.

## Regras técnicas atuais

- Carregar somente o necessário para a primeira tela; conteúdo abaixo da dobra deve ser lazy/on-demand.
- Animações de entrada só iniciam quando o conteúdo chega à viewport.
- Desktop com ponteiro fino pode usar rastros no hero; touch recebe somente o pulso de toque nas seções escuras.
- Respeitar `prefers-reduced-motion`.
- Preservar proporções de elementos decorativos com `aspect-ratio`, limites e overflow controlado.
- Enquanto o ponteiro estiver sobre um trilho do repertório, a roda controla exclusivamente o trilho; a página não deve escapar nos limites.
- A resposta inercial começa desde a primeira rolagem: roda para baixo desloca os objetos para cima e roda para cima desloca para baixo. O deslocamento é acumulativo, limitado e permanece onde parou até uma nova rolagem; não há retorno automático ao centro.
- Sobre a abertura preta, o menu não possui fundo. Assim que a seção clara alcança sua altura, ele recebe imediatamente uma barra preta sólida, sem transição ou atraso.
- Ao retornar para a abertura, o canvas é restaurado imediatamente à cena preta antes de a barra desaparecer, impedindo qualquer clarão ou fade claro atrás do menu.
- A barra usa altura compacta e fixa por breakpoint, com marca, links e idioma centralizados verticalmente.
- Os três quadros do manifesto mantêm rotações e posições assimétricas, usando proporção 4:5 apenas para impedir esticamento em qualquer viewport.
- O site possui conteúdo integral em português e inglês, alternado pelo botão de idioma sem recarregar a página.
- Não inventar URLs, contato ou projetos reais.

## Próxima organização

Quando entrarem novas rotas ou catálogo real, separar gradualmente:

- `src/styles/` para estilos globais e da disciplina;
- `src/scripts/` para canvas, reveals, exposição e contato;
- `src/content/design/` para dados versionados dos projetos;
- `public/media/` para imagens finais otimizadas.

A separação deve ser mecânica e validada visualmente; não é autorização para redesenhar a página.
