# GUIA DE MANUTENÇÃO DO LAYOUT APROVADO

## Referência visual definitiva
O arquivo **`LAYOUT_REFERENCE_APPROVED.png`** é a referência visual aprovada da página inicial.

## Regra principal
Para manter o layout exatamente como aprovado, **não altere**:
- `hero-map-photo-v10.jpg`
- o bloco CSS identificado como **`V10 — APPROVED LAYOUT LOCK`**
- as classes `hero-visual-v10`, `hero-transition-v10`, `approved-hero`, `approved-copy`
- as dimensões-base de 1536 × 458 px da área principal da Home

## Por que esta versão evita os erros anteriores
Nas versões anteriores, a imagem era usada como `background-size: cover`, o que cortava o Brasil ou ampliava a África.  
Nesta versão:
1. o mapa + retrato são carregados como uma imagem HTML normal;
2. a altura controla a escala;
3. a largura é automática;
4. a proporção original é preservada;
5. não existe `cover`, `fill` ou comando equivalente na imagem principal.

Isso impede:
- rosto esticado;
- corte excessivo do Brasil;
- zoom involuntário na África;
- deformação horizontal da fotografia.

## O que pode ser atualizado com segurança
Você pode editar:
- textos das páginas HTML;
- publicações;
- projetos;
- prêmios;
- links;
- e-mail;
- CV.

Para alterar apenas conteúdo textual, **não mexa em `styles.css`**.

## Upload no GitHub
1. Extraia este ZIP.
2. Abra o repositório `robsonpedrosacosta`.
3. Clique em **Add file → Upload files**.
4. Envie todos os arquivos desta pasta para a raiz do repositório.
5. Use a mensagem:
   `Lock approved homepage layout v10`
6. Clique em **Commit changes**.
7. Aguarde 1–3 minutos.
8. Abra:
   `https://robsonpc-alt.github.io/robsonpedrosacosta/?v=10`
9. Faça `Ctrl + F5` uma vez.

## IMPORTANTE
Não apague `LAYOUT_REFERENCE_APPROVED.png`.  
Mesmo que ela não apareça diretamente no site, ela serve como referência futura para comparar qualquer atualização com o layout aprovado.
