# Arthur — Design / Pictorial V08

Continuação direta da V07, sem troca da base visual.

Alterações desta rodada:
- removidos os textos instrucionais “passe o mouse + role” e “role para atravessar”;
- fundo inicial ganhou movimento sutil: granulação viva, atmosfera lenta e partículas;
- Arthur / Designer, laterais, kicker, CTA e indicação inferior agora entram com animação própria na abertura;
- objetos do contato ocupam a seção inteira e são conduzidos pelo mouse/toque com inércia, offsets e movimento autônomo; não fogem do cursor;
- interação dos objetos também responde a touch em celular;
- reforço responsivo para 1180 / 900 / 560 px, incluindo hero, decoração, quadros, repertório, exposição e contato;
- os trilhos de repertório continuam com swipe horizontal nativo em touch e wheel lateral em desktop.

QA executado em CSS viewports 1920x1080, 1440x900, 720x700, 390x844 e 320x568. Não houve overflow horizontal de documento nos tamanhos testados. Mouse e touch foram testados sobre os objetos do contato.
