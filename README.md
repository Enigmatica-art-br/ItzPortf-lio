# Arthur — Design / Pictorial V09

Continuação direta da V08, sem troca da base visual.

Alterações desta rodada:
- removidos os textos instrucionais “passe o mouse + role” e “role para atravessar”;
- fundo inicial ganhou movimento sutil: granulação viva, atmosfera lenta e partículas;
- Arthur / Designer, laterais, kicker, CTA e indicação inferior agora entram com animação própria na abertura;
- objetos do contato ocupam a seção inteira e são conduzidos pelo mouse/toque com inércia, offsets e movimento autônomo; não fogem do cursor;
- interação dos objetos também responde a touch em celular;
- reforço responsivo para 1180 / 900 / 560 px, incluindo hero, decoração, quadros, repertório, exposição e contato;
- os trilhos de repertório continuam com swipe horizontal nativo em touch e wheel lateral em desktop.

QA executado em CSS viewports 1920x1080, 1440x900, 720x700, 390x844 e 320x568. Não houve overflow horizontal de documento nos tamanhos testados. Mouse e touch foram testados sobre os objetos do contato.

## V09

- removida a elipse/"bola" que seguia o ponteiro no hero; no desktop permanecem apenas os rastros;
- clique/toque gera o mesmo pulso nas duas seções escuras: hero e contato;
- em dispositivos touch, rastros e feixes decorativos do hero ficam desligados;
- os três quadros do manifesto preservam proporção em mobile, zoom e viewports comprimidas;
- loading inicial curto espera somente os recursos críticos e tem limite de tempo;
- canvases das seções são criados sob demanda, com densidade e custo menores em dispositivos touch;
- o canvas deixa de ser redesenhado continuamente quando a cena está parada e pausa em aba oculta;
- imagens de destaque, exposição e cases usam decodificação assíncrona/lazy loading.
- bloco principal de contato centralizado na seção em desktop e mobile.
- proporções dos três quadros do manifesto e das quatro molduras de projetos travadas entre viewports;
- textos e objetos acumulam um deslocamento físico amortecido no sentido oposto à roda, proporcional à velocidade e limitado a 18 px; a posição permanece até uma nova rolagem;
- as molduras laranja e verde de Projetos em destaque foram reposicionadas para manter folga entre elas após as animações, sem sobreposição;
- a roda do mouse fica capturada pelo trilho de repertório enquanto o ponteiro estiver sobre ele, inclusive nos limites.
- sobre a abertura preta, a navegação compacta fica transparente; quando a seção clara alcança o menu, ela troca instantaneamente para uma barra preta sólida, sem fade ou atraso;
- os três quadros do manifesto preservam a composição torta e assimétrica, mas usam proporção fixa 4:5 para não deformar entre desktop e celular;
- o seletor PT/EN traduz toda a interface, os textos editoriais, categorias, descrições e painéis de projeto nos dois sentidos.

O projeto continua deliberadamente sem framework nesta fase visual. Antes de novas rotas ou conteúdo real, o próximo passo estrutural é separar estilos, interações e catálogo de projetos sem reescrever a linguagem visual aprovada.
