# Site da Academia UDI-U01

Documento de referência para construir o site da **Academia UDI-U01**, programa de capacitação com o Kiro da **SL23 Treinamentos** para alunos e egressos da Universidade Federal de Uberlândia (UFU). Ele define objetivo, público, marcas, layout no padrão do portal da UFU, ilustrações, estrutura das seções com os textos finais, comportamento dos componentes e pendências antes da publicação. O arquivo `modelo-site-programa-kiro-ufu.html` é a implementação visual destas instruções.

## 1. Objetivo do site

Apresentar a Academia UDI-U01, explicar como o programa funciona e levar o visitante a duas ações:

1. **Saiba mais sobre o programa**: ação principal, leva à seção de perguntas e contato.
2. **Manifestar interesse**: leva ao formulário de inscrição.

## 2. Público

| Público | O que precisa encontrar |
|---|---|
| Alunos de graduação e pós-graduação da UFU | Como participar, carga horária, o que vão aprender e construir |
| Egressos da UFU que atuam como desenvolvedores | Valor prático para o trabalho e formato compatível com a rotina |
| Professores e coordenação da FACOM | Formato acadêmico, papel da UFU e acompanhamento |
| Empresas da região | Demo Day, perfil dos participantes e possibilidade de levar o método para dentro da empresa |
| AWS | Escopo, parceria e resultados esperados |

## 3. Título e mensagem central

- **Título do site:** Academia UDI-U01
- **Marca no topo:** SL23 Treinamentos
- **Mensagem:** Aprenda a construir software com IA começando pela especificação.

Fatos que precisam aparecer no site, sempre com estes números:

- 50 vagas para alunos e egressos da UFU
- 4 aulas presenciais de 4 horas (16 horas de aula)
- 90 dias de programa, com projetos em equipe entre as aulas
- Aulas nos laboratórios da UFU
- Aulas ministradas por profissionais da UFU e da Núvoli
- Acesso ao Kiro no plano Kiro Power durante os 90 dias
- Um projeto por equipe implantado na AWS e apresentado no Demo Day

## 4. Marcas e logotipos

| Marca | Arquivo | Onde aparece | Aplicação |
|---|---|---|---|
| SL23 Treinamentos | `sl23-treinamentos-logo.svg` (versão branca: `sl23-treinamentos-logo-branca.svg`) | **Canto superior esquerdo do cabeçalho**, em todas as telas; também nas imagens das aulas | Altura de 46 px no desktop e 37 px no celular |
| UFU | `https://ufu.br/themes/custom/ufu/logo.svg` (cor `#3B3174`) | **Somente na seção Parceria** | Primeiro na ordem de leitura, ao lado da Núvoli |
| Núvoli | Logotipo oficial para fundo claro | **Somente na seção Parceria** | Depois da UFU, separados por divisor vertical |
| AWS | Logotipo do cabeçalho de `aws.amazon.com` (SVG monocromático, cor `#232F3E`) | Logo abaixo do cartão "Ficou alguma dúvida?", com o rótulo "Apoio" | Pequeno, com 21 px de altura |

### 4.1 Logotipo SL23 Treinamentos

- **Símbolo:** quadrado de cantos arredondados em azul `#155BCB` com uma escada branca de três degraus e um ponto âmbar `#F2B705` no degrau mais alto. A escada representa a evolução do aluno ao longo do treinamento; o ponto, o objetivo alcançado.
- **Texto:** "SL23" em Noto Sans Black, azul marinho `#071D41`, e "Treinamentos" em Noto Sans Medium, azul `#155BCB`. Na versão branca, "SL23" em branco e "Treinamentos" em `#9EC0F5`.
- **Arquivos:** SVG com o texto convertido em curvas (não depende de fonte instalada) e PNG com fundo transparente.
- **Tamanho mínimo:** 32 px de altura em tela.
- **Área de proteção:** metade da altura do símbolo em todos os lados.

### 4.2 Regras da marca UFU

- Quando aparece com outras marcas, a UFU vem primeiro na ordem de leitura, conforme o manual de aplicação da marca.
- Tamanho mínimo da assinatura horizontal principal: 49,2 px (1,3 cm) de altura.
- **Autorização obrigatória:** pela Resolução 04/2011 do Conselho Universitário (art. 5º), empresas externas só podem usar a marca UFU com autorização da Reitoria, formalizada em contrato escrito de licenciamento ou cessão de uso não exclusivo.

### 4.3 Regras da marca Núvoli

- O logotipo da Núvoli aparece apenas na seção Parceria. Nas demais seções, a Núvoli é citada só em texto.

### 4.4 Regras do apoio AWS

- Logotipo pequeno, apenas uma vez, abaixo do cartão "Ficou alguma dúvida?".
- Antes de publicar, confirmar com a AWS a aprovação da menção de apoio e substituir o arquivo pelo selo indicado no Partner Central, se a AWS assim orientar.
- Os nomes de serviços AWS aparecem sempre por extenso e em texto, nunca como logotipos.

## 5. Layout

### 5.1 Elementos no padrão do portal UFU

| Elemento do portal `ufu.br` | Como aparece no site |
|---|---|
| Cabeçalho branco com menu hambúrguer à esquerda | Igual, com o logotipo SL23 Treinamentos e, ao lado, "Academia UDI-U01" e "Programa de Capacitação Kiro" |
| Controles de acessibilidade no canto superior direito | A-, A, A+ e contraste, funcionando |
| Linha de botões em pílula com contorno azul | Atalhos para O método, Como funciona, Para quem é, Parceria e Saiba mais |
| Banner de destaque com cantos arredondados | Banner azul marinho com o título "Academia UDI-U01" e o cartão de especificação |
| Títulos de seção centralizados, em caixa alta, com filetes laterais | Igual em todas as seções |
| Bloco "Acesso rápido" | Quatro blocos com os números do programa |
| Cartões de notícia com imagem, categoria e título em azul | Cartões das 4 aulas com as ilustrações |

### 5.2 Elementos que não entram

- **Rodapé azul do portal:** removido. A página termina na seção Saiba mais sobre o programa, com o cartão "Ficou alguma dúvida?" e o apoio AWS.
- **Barra do governo federal (gov.br)** e "Ministério da Educação": identificam páginas oficiais do governo.
- Busca geral, menus institucionais e selo de Acesso à Informação do portal.

### 5.3 Paleta

| Nome | Hex | Uso |
|---|---|---|
| Azul | `#155BCB` | Links, botões, títulos de cartões, símbolo SL23 |
| Azul escuro | `#0F47A3` | Passagem do mouse nos botões |
| Marinho | `#071D41` | Banner, fundo das ilustrações, texto "SL23" |
| Azul claro | `#9EC0F5` | Detalhes das ilustrações e textos sobre fundo escuro |
| Âmbar | `#F2B705` | Destaques das ilustrações, ponto do símbolo SL23, contorno de foco |
| Texto | `#212529` | Texto principal e filetes dos títulos |
| Texto secundário | `#495057` | Descrições |
| Cinza claro | `#F5F7FA` | Fundo das seções alternadas |
| Linha | `#DEE2E6` | Bordas |

### 5.4 Tipografia

- **Noto Sans** em todos os textos (400 a 700); **Noto Sans Mono** apenas no cartão de especificação.
- Título do banner "Academia UDI-U01": 50 px, peso 700 (34 px no celular, sem quebrar "UDI-U01").
- Frase de apoio do banner: 25 px, peso 500.
- Títulos de seção: 32 px, peso 500, caixa alta.

## 6. Ilustrações das aulas

Quatro ilustrações originais em estilo plano, no fundo marinho com grade sutil e luz azul, usando apenas a paleta do site. Cada uma mostra o tema da aula sem logotipos de terceiros nem ícones de serviços AWS.

| Aula | Cena | Arquivos |
|---|---|---|
| Aula 1: fundamentos do Kiro e da especificação | Lâmpada acesa (a ideia) com seta para um documento de requisitos e uma lista de tarefas com três itens marcados | `aula1.svg` (cartão do site) e `academia-udi-u01-aula-1.png` |
| Aula 2: construção na AWS | Janela de código com `</>` e engrenagem (hooks) enviando blocos que se empilham dentro de uma nuvem | `aula2.svg` e `academia-udi-u01-aula-2.png` |
| Aula 3: IA generativa com Amazon Bedrock | Balão de conversa, rede de nós com centro âmbar e três pequenos agentes conectados (subagentes) | `aula3.svg` e `academia-udi-u01-aula-3.png` |
| Aula 4: Demo Day | Tela de apresentação com gráfico em alta, estrela de destaque, feixe de luz e plateia | `aula4.svg` e `academia-udi-u01-aula-4.png` |

- **No site:** as ilustrações ocupam a capa de cada cartão (16:9), com degradê escuro na base e o texto "Aula N" e a carga horária no canto inferior esquerdo.
- **Imagens avulsas (PNG 1600 x 900):** para redes sociais e apresentações, com o logotipo SL23 branco no canto superior esquerdo e, no canto inferior esquerdo, "Academia UDI-U01", "Aula N", o tema e a semana.

## 7. Estrutura e textos

Página única com navegação por âncoras.

| Ordem | Âncora | Seção |
|---|---|---|
| 1 | | Cabeçalho, menu lateral e linha de pílulas |
| 2 | `#programa` | Banner de destaque |
| 3 | | Acesso rápido |
| 4 | `#metodo` | O método |
| 5 | `#como-funciona` | Como funciona |
| 6 | `#onde` | Onde e com quem |
| 7 | `#para-quem` | Para quem é |
| 8 | `#projetos` | O que você vai construir |
| 9 | `#parceria` | Parceria |
| 10 | `#saiba-mais` | Saiba mais sobre o programa, com o apoio AWS ao final |

### 7.1 Cabeçalho

- Esquerda: menu hambúrguer, logotipo SL23 Treinamentos e, separado por um filete, **Academia UDI-U01** com "Programa de Capacitação Kiro" abaixo.
- Direita: "Acessibilidade A- A A+" e contraste; abaixo, botão **Saiba mais sobre o programa**.
- O menu hambúrguer abre um painel lateral com todas as seções.
- Abaixo do cabeçalho, linha de pílulas: O método, Como funciona, Para quem é, Parceria, Saiba mais.
- No celular: hambúrguer, logotipo SL23 e acessibilidade; as pílulas rolam na horizontal.

### 7.2 Banner de destaque

- **Categoria:** Programa de capacitação com o Kiro
- **Título:** Academia UDI-U01
- **Frase:** Aprenda a construir software com IA começando pela especificação.
- **Texto:** Para alunos e egressos da UFU: 4 aulas nos laboratórios da universidade, 90 dias de prática em equipe e um projeto real implantado na AWS.
- **Botões:** Saiba mais sobre o programa (branco) e Manifestar interesse (contorno branco).
- **Cartão de especificação** à direita (abaixo no celular):

```
programa-kiro-ufu/requirements.md

Requisito 1. Formação
QUANDO o participante concluir as 4 aulas
ENTÃO ele DEVE transformar uma ideia em requisitos, design e tarefas

Requisito 2. Prática
ENQUANTO o programa durar 90 dias
CADA equipe DEVE construir e implantar um projeto na AWS

Requisito 3. Mercado
QUANDO o participante voltar ao estágio ou ao trabalho
ENTÃO ele DEVE conseguir apresentar o método à empresa

tasks.md
[ ] Aula 1: fundamentos do Kiro e da especificação
[ ] Aula 2: construção na AWS
[ ] Aula 3: IA generativa com Amazon Bedrock
[ ] Aula 4: Demo Day
```

As tarefas são marcadas uma a uma quando a página carrega (único movimento automático do site).

### 7.3 Acesso rápido

Quatro blocos: **50** vagas para alunos e egressos; **16 h** de aula em 4 encontros; **90 dias** de programa com projeto; **Kiro Power** durante todo o programa.

### 7.4 O método

**Texto:** O Kiro é o agente de IA da AWS para engenharia de software. Em vez de gerar código a partir de um pedido solto, ele organiza o trabalho em etapas que você revisa e aprova.

1. **Requisitos:** a ideia vira comportamentos verificáveis, escritos de forma que qualquer pessoa da equipe entenda.
2. **Design:** o Kiro propõe a arquitetura, os dados e as interfaces, e você ajusta antes de seguir.
3. **Tarefas:** o design vira uma lista ordenada de tarefas pequenas, cada uma ligada a um requisito.
4. **Código e testes:** o agente executa as tarefas, gera testes e você confere se o resultado cumpre a especificação.

**Nota:** No programa você também usa hooks, que automatizam testes e documentação, steering, que guarda as regras do projeto, e subagentes, que dividem o trabalho em frentes paralelas.

### 7.5 Como funciona

**Texto:** São 90 dias, 4 aulas e um projeto do começo ao fim. As aulas ensinam o método; entre elas, sua equipe aplica o que aprendeu com acompanhamento dos instrutores.

| Capa (ilustração) | Categoria | Título | Descrição |
|---|---|---|---|
| Aula 1, 4 horas no laboratório | Semana 1 | Fundamentos do Kiro e da especificação | Formação das equipes, escolha do problema e primeira especificação completa. |
| Aula 2, 4 horas no laboratório | Semana 5 | Construção na AWS | Serverless, infraestrutura como código e hooks para testes automáticos. |
| Aula 3, 4 horas no laboratório | Semana 9 | IA generativa com Amazon Bedrock | Subagentes, logs, alarmes e prontidão para produção. |
| Aula 4, 4 horas de Demo Day | Semana 12 | Demo Day | Banca com profissionais da UFU, da Núvoli e de empresas convidadas. |

Abaixo, linha do tempo de 13 semanas (oculta no celular) e a frase: "Entre os encontros há plantões quinzenais e um canal permanente de dúvidas."

### 7.6 Onde e com quem

- **Nos laboratórios da UFU:** As aulas acontecem em [laboratório e campus]. Entre os encontros, você pode trabalhar no laboratório, no seu computador ou no Kiro Web, que roda no navegador.
- **Com profissionais da UFU e da Núvoli:** As aulas são conduzidas por profissionais da UFU e da Núvoli, parceira AWS em Uberlândia. Os instrutores acompanham cada equipe do primeiro requisito ao Demo Day.

### 7.7 Para quem é

**Texto:** Para quem já programa e quer trabalhar do jeito que as empresas estão adotando.

- Ser aluno de graduação ou pós-graduação da UFU, ou egresso da universidade.
- Saber programar em pelo menos uma linguagem.
- Ter disponibilidade para as 4 aulas presenciais e para o projeto em equipe.
- Prioridade para quem estagia ou trabalha em empresas da região.

### 7.8 O que você vai construir

**Texto:** Cada equipe de 5 pessoas escolhe um problema, escreve a especificação e entrega uma aplicação funcionando em conta AWS. São 10 equipes e 10 projetos apresentados no Demo Day.

Serviços em pílulas de texto: Amazon Bedrock, AWS Lambda, Amazon API Gateway, Amazon DynamoDB, Amazon S3, AWS Cloud Development Kit e Amazon CloudWatch. Ao lado, diagrama da arquitetura de referência.

### 7.9 Parceria

Logotipos UFU e Núvoli, nesta ordem, centralizados. **Única seção com esses dois logotipos.**

- **Universidade Federal de Uberlândia:** Oferece os laboratórios, participa das aulas com seus profissionais e faz o acompanhamento acadêmico, por meio da Faculdade de Computação.
- **Núvoli:** Parceira AWS em Uberlândia, conduz aulas, prepara o ambiente na AWS, gerencia as licenças do Kiro e acompanha as equipes entre os encontros.

### 7.10 Saiba mais sobre o programa (fim da página)

Perguntas frequentes em acordeão:

- **Quem pode participar?** Alunos de graduação e pós-graduação da UFU e egressos que atuam como desenvolvedores. São 50 vagas.
- **O programa tem custo?** Não há custo para os participantes.
- **Quanto tempo vou dedicar?** São 16 horas de aula, em 4 encontros de 4 horas, mais o trabalho do projeto em equipe ao longo dos 90 dias.
- **Preciso ter computador próprio?** Não. As aulas acontecem nos laboratórios da UFU e o Kiro Web roda no navegador. Se tiver computador, você também pode usá-lo.
- **Recebo certificado?** Sim, com presença mínima de 75% nas aulas e participação nas entregas da equipe.
- **Posso usar código da empresa onde estagio?** Não. Os projetos usam dados fictícios ou públicos. Código e dados de empresas só com autorização formal delas.
- **Como faço para participar?** Preencha o formulário de manifestação de interesse até [data limite]. A seleção considera os requisitos da seção Para quem é.

Ao lado das perguntas (abaixo delas no celular):

1. **Cartão azul "Ficou alguma dúvida?"**: texto "Fale com a coordenação do programa ou deixe seu interesse registrado para a seleção.", botões **Manifestar interesse** e **Enviar mensagem**, o e-mail [e-mail de contato do programa] e o link "Política de privacidade".
2. **Apoio AWS**, logo abaixo do cartão: rótulo "Apoio" e o logotipo AWS pequeno. **É o último elemento da página; não há rodapé.**

## 8. Componentes e comportamento

- **Botões:** formato pílula. Principal com fundo azul; no banner e no cartão de contato, versões branca e com contorno branco.
- **Acessibilidade:** A- e A+ mudam o tamanho de todo o texto; A volta ao padrão; contraste aplica fundo preto, texto branco e links amarelos (o logotipo SL23 é invertido nesse modo).
- **Menu lateral:** abre pelo hambúrguer e fecha pelo botão "Fechar menu", pela tecla Esc ou clicando fora.
- **Acordeão:** elementos `details` e `summary`, funcionando por teclado.
- **Foco:** contorno âmbar de 3 px em todos os elementos interativos.
- **Link "Ir para o conteúdo"** no início da página, visível ao receber foco.
- **Movimento:** apenas a marcação das tarefas no banner; respeitar `prefers-reduced-motion`.
- **Responsivo:** uma coluna abaixo de 900 px, margem lateral de 16 px, sem rolagem horizontal.
- **Texto alternativo:** logotipos ("SL23 Treinamentos", "Universidade Federal de Uberlândia", "Núvoli", "Amazon Web Services") e descrição de cada ilustração de aula.

## 9. SEO e compartilhamento

- **Título da página:** Academia UDI-U01 | Programa de Capacitação Kiro
- **Descrição:** Programa de capacitação com o Kiro para alunos e egressos da UFU: 4 aulas nos laboratórios da universidade, 90 dias de prática e um projeto implantado na AWS.
- **Imagem de compartilhamento:** usar `academia-udi-u01-aula-1.png` ou uma versão 1200 x 630 com o título do programa e o logotipo SL23.
- **Idioma:** `pt-BR`.

## 10. Formulário de manifestação de interesse

Campos: nome completo, e-mail institucional ou pessoal, vínculo com a UFU (graduação, pós-graduação ou egresso), curso, empresa onde estagia ou trabalha (opcional), experiência com programação, disponibilidade para as 4 aulas.

Incluir aviso de privacidade conforme a LGPD (Lei 13.709/2018): finalidade exclusiva de seleção e comunicação do programa, e canal para solicitar exclusão dos dados.

## 11. Hospedagem sugerida

AWS Amplify Hosting ou Amazon S3 com Amazon CloudFront, com certificado TLS e domínio da SL23 Treinamentos.

## 12. Pendências antes da publicação

| Item | Responsável |
|---|---|
| Autorização da Reitoria para uso da marca UFU na seção Parceria (Resolução 04/2011, art. 5º) | SL23, Núvoli e FACOM |
| Aprovação da AWS para a menção de apoio e confirmação do arquivo de logotipo | Núvoli |
| Definir se a SL23 Treinamentos entra no texto da seção Parceria | SL23 |
| Liberação das licenças Kiro Power pela AWS | AWS |
| Laboratório e campus das aulas | FACOM |
| Datas das 4 aulas e prazo de inscrição | SL23 e FACOM |
| Link do formulário, e-mail de contato e política de privacidade | SL23 |
| Nomes dos instrutores, se forem divulgados | SL23, Núvoli e FACOM |
