# Documento de planeamento — | NortePet

## 1. Identificação
- **Projeto:** NortePet — serviço fictício de pet sitting e visitas ao domicílio.
- **Público-alvo:** pessoas de Vila Nova de Gaia que necessitam de apoio temporário para cuidar dos seus animais de companhia.
- **Objetivo geral:** criar um sítio Web estático, acessível e fácil de navegar, que apresente os serviços fictícios e permita consultar informações e preencher um formulário de contacto de demonstração.

## 2. Objetivos por etapa

### Análise
- Identificar as necessidades do público-alvo e a informação que procura.
- Definir os conteúdos essenciais: apresentação, serviços, contacto, artigo e declaração de acessibilidade.
- Analisar requisitos de semântica HTML, acessibilidade, validação e navegação.
- **Resultado esperado:** requisitos e público-alvo documentados no README e no mapa do sítio.

### Planeamento
- Organizar as páginas e as ligações internas no sitemap.
- Definir tarefas, ordem de implementação e evidências a guardar para cada entrega.
- Estabelecer critérios de verificação: um `h1` por página, estrutura semântica, rótulos associados e validação HTML5.
- **Resultado esperado:** sitemap atualizado, documento de planeamento e checklist E2.

### Desenho
- Usar os wireframes de baixa fidelidade da E1 como base para a estrutura das páginas.
- Manter cabeçalho, navegação e rodapé coerentes em todas as páginas.
- Organizar o formulário por campos com rótulos claros, instruções e mensagens de ajuda.
- **Resultado esperado:** estrutura previsível e consistente, preparada para receber a folha de estilos numa entrega posterior.

### Implementação
- Completar as páginas Início, Serviços e Contacto e criar as páginas Artigo e Acessibilidade.
- Utilizar elementos semânticos (`header`, `nav`, `main`, `section`, `article` e `footer`) e um único `h1` por página.
- Criar formulário de contacto com diferentes controlos, `label` associado a cada controlo e validação nativa (`required`, `type`, `pattern`, `minlength` e `maxlength`).
- Verificar caminhos das imagens e ligações internas.
- **Resultado esperado:** cinco páginas HTML completas e formulário de demonstração. Nesta fase, o formulário não envia dados para um servidor.

### Marketing e publicação
- Comunicar a proposta fictícia da NortePet através de texto simples e ligações claras para os serviços e contacto.
- Preparar títulos e descrições únicos para cada página, favorecendo a identificação do conteúdo nos motores de pesquisa.
- Numa fase posterior, publicar o sítio num endereço público e divulgar o URL em canais adequados ao público-alvo.
- **Resultado esperado:** conteúdos preparados para divulgação; a publicação pública será feita numa entrega posterior.

## 3. Organização das páginas
| Página | Objetivo |
|---|---|
| `index.html` | Apresentar a NortePet e encaminhar para os conteúdos principais. |
| `servicos.html` | Descrever os serviços fictícios e apresentar uma tabela-resumo. |
| `contacto.html` | Mostrar informações de exemplo e recolher dados num formulário de demonstração. |
| `artigo.html` | Publicar um texto informativo relacionado com os cuidados dos animais. |
| `acessibilidade.html` | Descrever as medidas de acessibilidade consideradas e as limitações atuais. |

## 4. Critérios de verificação da E2
1. Documento de planeamento com objetivos das etapas de análise, planeamento, desenho, implementação e marketing.
2. Cinco páginas HTML com estrutura semântica, navegação comum e um único `h1` por página.
3. Formulário com seis ou mais tipos de controlo e `label` associado a cada controlo.
4. Validação nativa HTML5 aplicada aos campos relevantes.
5. Todas as páginas verificadas no validador HTML do W3C; guardar captura/relatório após validação.

## 5. Limitações conhecidas
O projeto é fictício e não existe backend. O formulário serve para demonstrar estrutura e validação do lado do navegador, não para enviar pedidos reais. A folha de estilos, o teste de contraste e a auditoria de acessibilidade serão desenvolvidos em entregas seguintes.
