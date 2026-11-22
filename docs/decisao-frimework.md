# Decisão da framework CSS — NortePet

**Decisão:** NortePet continua a usar o **Bootstrap 5.3.9**.

## Porquê

A comparação do componente Card está em `comparacao.html`. Os dados que pesaram:

- **Documentação:** Bootstrap 8/10, Foundation 6/10, W3.CSS 5/10. Só o Bootstrap tem pesquisa, barra lateral, secção de personalização e nota de acessibilidade na página do Card. Num projeto de grupo, documentação clara reduz erros e tempo.
- **Personalização:** igualar o guia de estilo do NortePet (#176B5B, cantos de 8 px, borda #CBD5D1) custou 2 linhas de CSS no Bootstrap, contra 3 no Foundation e 3 no W3.CSS. O Bootstrap usa variáveis CSS e não precisou de `!important`; o W3.CSS precisou.
- **Acessibilidade por defeito:** Lighthouse 100 no Bootstrap e no Foundation, 90 no W3.CSS (contraste insuficiente).
- **Custo de migração:** o Bootstrap já está nas 5 páginas, com 4 componentes (Alert, Button, Card, List Group), grelhas em Início e Serviços e 5 personalizações. Mudar obrigaria a refazer tudo. Este argumento é secundário e não decide sozinho.

## O que perdemos

O Bootstrap é a opção mais pesada: **23,1 kB** de CSS, contra 14,8 kB no Foundation (+8,3 kB) e 6,1 kB no W3.CSS (+17,0 kB). Nenhum dos três carregou JavaScript no componente comparado. Num sítio estático e pequeno, esta diferença é aceitável, mas existe.

## Impacto no sítio final

- Mantêm-se o Bootstrap por CDN, o `estilos.css` e o `bootstrap-personalizado.css`, sem alterar o código da framework.
- O Foundation e o W3.CSS ficam apenas nas demonstrações da pasta `comparacao/`, fora do sítio final.
- Não há migração.

## Riscos e mitigação

- **Peso do CSS:** carregar apenas o CSS (sem o JavaScript do Bootstrap, que o sítio não usa) e comprimir as imagens grandes, que pesam mais do que a framework.
- **Aspeto genérico:** manter as personalizações do guia de estilo.
- **Dependência da CDN:** a versão está fixa (5.3.9) e com verificação de integridade (SRI).
