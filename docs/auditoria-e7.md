# Relatório de Auditoria — E7

## Projeto NortePet
Unidade Curricular: Programação Web - Cliente

Data: 22/11/2026

## 1. Objetivo

Corrigir os problemas identificados na
auditoria E6 e verificar o resultado
com a mesma ferramenta.

## 2. Problemas da auditoria E6

A auditoria E6 (docs/auditoria-E6.md)
identificou um único tipo de problema:

- 3 alertas "Redundant Link" (WAVE) na
  página inicial (index.html).

O Lighthouse (Acessibilidade e SEO) deu
100/100 nas três páginas analisadas, e o
WAVE não registou erros nem erros de
contraste.

Total de problemas da E6: 3.

## 3. Correções aplicadas (index.html)

Os alertas indicam ligações vizinhas
com o mesmo destino. Foram aplicadas
estas três correções:

| # | Ligações redundantes | Correção |
|---|---|---|
| 1 | Logótipo (index.html) seguido de "Início" no menu (index.html) | Na página inicial, o logótipo deixou de ser ligação. O texto alternativo passou a "NortePet". |
| 2 | "formulário de contacto" (contacto.html) seguido do botão "Pedir informações" (contacto.html) | A ligação no texto passou a texto simples. O botão mantém-se. |
| 3 | "entrar em contacto" (contacto.html) seguido de "Contactos" no rodapé (contacto.html) | A ligação "entrar em contacto" foi removida do parágrafo dos serviços. |

## 4. Resultado depois das correções

Ferramenta: WAVE (wave.webaim.org).

| | Antes (E6) | Depois (E7) |
|---|---|---|
| Alertas "Redundant Link" | 3 | ___ |
| Erros | 0 | ___ |
| Erros de contraste | 0 | ___ |

Problemas corrigidos: ___ de 3 (___%).

Objetivo da E7: 80% ou mais.

## 5. Evidências

- docs/auditoria-E7/wave-index-antes.png
- docs/auditoria-E7/wave-index-depois.png

## 6. Conclusão

As três ligações redundantes da página
inicial foram corrigidas. O resultado
foi verificado com o WAVE.

As ferramentas automáticas não garantem
conformidade integral com as WCAG,
pelo que continuam a ser necessários
testes manuais.

