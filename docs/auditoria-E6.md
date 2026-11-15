
# Relatório de Auditoria — E6

## Projeto NortePet
Unidade Curricular: Programação Web - Cliente

Data: 15/11/2026

## 1. Objetivo

Avaliar a acessibilidade e o SEO do site
NortePet, identificando problemas e
definindo um plano de correção.

## 2. Ferramentas utilizadas

- Google Lighthouse (modo Mobile)
- WAVE — Web Accessibility Evaluation Tool

## 3. Páginas analisadas

- index.html — Página inicial
- servicos.html — Serviços
- contacto.html — Contacto

## 4. Resultados Lighthouse

| Página | Acessibilidade | SEO |
|---|---|---|
| Início | 100/100 | 100/100 |
| Serviços | 100/100 | 100/100 |
| Contacto | 100/100 | 100/100 |

As três páginas obtiveram pontuação
máxima nas categorias avaliadas.

## 5. Resultados WAVE

| Página | Errors | Contrast Errors | Alerts |
|---|---|---|---|
| Início | 0 | 0 | 3 |
| Serviços | 0 | 0 | 0 |
| Contacto | 0 | 0 | 0 |

## 6. Problemas identificados

O WAVE identificou três alertas do tipo
"Redundant Link" na página inicial.

Estes alertas indicam a existência de
ligações próximas que apontam para o
mesmo destino.

Não foram identificados erros automáticos
nem erros de contraste nas três páginas.

Os alertas requerem verificação manual,
mas não representam necessariamente
violações das normas de acessibilidade.

## 7. Plano de correção

### Problema 1 — Ligações redundantes

Página: index.html

Quantidade: 3 alertas

Ação prevista:
- Identificar as ligações assinaladas.
- Verificar se a repetição é necessária.
- Remover ou reorganizar ligações
  desnecessárias, quando adequado.
- Manter as ligações úteis à navegação.
- Repetir a auditoria WAVE.

Prioridade: Baixa, sujeita a revisão manual.

### Verificações complementares

- Confirmar a navegação por teclado.
- Verificar os textos alternativos.
- Testar a utilização dos formulários.
- Confirmar a apresentação em dispositivos
  móveis.

## 8. Evidências

Ferramentas:
- https://developer.chrome.com/docs/lighthouse/
- https://wave.webaim.org/

As capturas dos relatórios devem ser
guardadas na pasta docs/auditoria-E6/.

## 9. Conclusão

A auditoria inicial apresentou resultados
positivos nas três páginas analisadas.

O Lighthouse atribuiu 100 pontos nas
categorias de Acessibilidade e SEO.

O WAVE não identificou erros automáticos
nem problemas de contraste.

Foram identificados três alertas de
ligações redundantes na página inicial,
que serão analisados manualmente.

As ferramentas automáticas não garantem
conformidade integral com as WCAG,
pelo que são necessários testes manuais.
