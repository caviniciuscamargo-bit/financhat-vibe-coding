# financhat-vibe-coding
# FinanChat — Organização Financeira por Conversa

## Sobre o projeto

O FinanChat é o conceito de um aplicativo de organização de finanças pessoais que permite registrar receitas, despesas e metas usando linguagem natural.

Em vez de preencher formulários complexos, o usuário pode conversar com um Agente Financeiro usando mensagens como:

> “Gastei R$ 40 em uma hamburgueria.”

O aplicativo interpreta a mensagem, identifica o valor, a categoria e a subcategoria e apresenta os dados para confirmação antes de salvar.

O projeto também simula a identificação de gastos por meio de notificações bancárias recebidas no celular.

## Problema

Muitas pessoas querem organizar suas finanças, mas abandonam planilhas e aplicativos porque precisam:

- registrar cada gasto manualmente;
- preencher muitos campos;
- escolher categorias;
- atualizar os dados constantemente;
- interpretar relatórios complexos.

Além disso, pequenas compras acabam sendo esquecidas, prejudicando a visão real dos gastos mensais.

## Solução

O FinanChat propõe uma experiência simples e conversacional.

O usuário pode:

- registrar gastos e receitas pelo chat;
- confirmar gastos identificados em notificações;
- acompanhar movimentações;
- visualizar um resumo financeiro;
- criar metas;
- receber orientações educativas de um Agente Financeiro.

## Principal diferencial

O principal diferencial do FinanChat é reduzir o trabalho manual.

Em uma versão futura, o sistema poderá identificar notificações como:

> “Compra aprovada: R$ 42,90 — Supermercado Central.”

Depois, o aplicativo perguntará:

> “Identifiquei uma compra de R$ 42,90 no Supermercado Central. Deseja registrar como Alimentação?”

O usuário sempre poderá confirmar, editar, alterar a categoria ou ignorar a movimentação.

## Público-alvo

O projeto foi pensado principalmente para:

- pessoas que estão começando a organizar suas finanças;
- estudantes e trabalhadores;
- usuários que não utilizam planilhas;
- pessoas que abandonaram aplicativos financeiros;
- usuários que preferem conversar em vez de preencher formulários.

## Funcionalidades do MVP

- Registro de gastos por conversa.
- Registro de receitas.
- Classificação automática de movimentações.
- Categorias e subcategorias.
- Confirmação antes de salvar.
- Histórico de movimentações.
- Painel com receitas, despesas e saldo.
- Criação e acompanhamento de metas.
- Recomendações do Agente Financeiro.
- Simulação de notificações bancárias.
- Área de privacidade e permissões.

## Exemplo de funcionamento

### Mensagem do usuário

> Gastei R$ 40 em uma hamburgueria.

### Interpretação do FinanChat

- Tipo: Despesa
- Valor: R$ 40,00
- Categoria: Alimentação
- Subcategoria: Restaurante e lanche
- Estabelecimento: Hamburgueria
- Confiança: Alta

Antes de registrar, o aplicativo apresenta as opções:

- Salvar;
- Editar;
- Cancelar.

## Fluxo principal

1. O usuário acessa o aplicativo.
2. Visualiza o resumo do mês.
3. Abre o chat.
4. Digita uma movimentação financeira.
5. O agente interpreta a mensagem.
6. O usuário confirma ou corrige os dados.
7. A movimentação aparece no histórico.
8. O painel financeiro é atualizado.
9. O agente pode apresentar uma orientação.
10. O usuário acompanha suas metas financeiras.

## Telas desenvolvidas

### Página inicial

Apresenta:

- saldo estimado;
- receitas;
- despesas;
- resultado do mês;
- meta principal;
- categorias com maiores gastos;
- movimentações recentes.

### Chat

Permite registrar receitas, despesas e metas usando linguagem natural.

### Movimentações

Apresenta o histórico financeiro, incluindo:

- descrição;
- valor;
- categoria;
- data;
- origem do registro.

### Metas

Permite acompanhar:

- valor total da meta;
- valor economizado;
- valor restante;
- percentual concluído;
- prazo;
- valor mensal recomendado.

### Perfil e privacidade

Explica:

- quais permissões seriam utilizadas;
- quais aplicativos bancários estariam autorizados;
- quais informações seriam processadas;
- o que o FinanChat não realiza;
- como o usuário pode desativar as notificações.

## Capturas do protótipo

### Página inicial

![Página inicial do FinanChat](imagens/inicio.png)

### Registro por conversa

![Chat do FinanChat](imagens/chat.png)

### Histórico de movimentações

![Histórico do FinanChat](imagens/movimentacoes.png)

### Metas financeiras

![Metas do FinanChat](imagens/metas.png)

### Privacidade e permissões

![Privacidade do FinanChat](imagens/privacidade.png)

## Ferramentas utilizadas

- ChatGPT para elaboração e revisão do PRD.
- Lovable para criação do protótipo visual.
- GitHub para documentação e apresentação.
- Conceitos de Vibe Coding.
- Conceitos de Produto Mínimo Viável.
- Engenharia de prompts.

## Vibe Coding

O projeto foi desenvolvido utilizando os princípios de Vibe Coding.

Em vez de escrever o código manualmente, o processo começou com a descrição detalhada:

- do problema;
- do público-alvo;
- das funcionalidades;
- das regras de negócio;
- das telas;
- do comportamento do agente;
- das limitações do produto.

A inteligência artificial foi utilizada como parceira para transformar essas instruções em um protótipo navegável.

## Testes realizados

Durante os testes, foram utilizadas mensagens como:

- “Gastei R$ 40 em uma hamburgueria.”
- “Paguei R$ 22 na padaria.”
- “Recebi R$ 300 de um trabalho extra.”
- “Gastei R$ 34 em um Uber para o trabalho.”

O sistema conseguiu diferenciar:

- receitas;
- despesas;
- alimentação;
- transporte;
- lazer;
- outras categorias.

## Problema encontrado durante os testes

Em uma das primeiras versões, a mensagem:

> “Gastei R$ 30 em uma hamburgueria.”

foi classificada como “Outros”.

Depois da revisão do prompt, o sistema passou a apresentar:

- Categoria: Alimentação;
- Subcategoria: Restaurante e lanche;
- Confiança: Alta.

Esse teste mostrou que a inteligência artificial precisa receber contexto, exemplos e regras claras para produzir classificações mais confiáveis.

Também foi identificado que uma movimentação de farmácia apareceu classificada como “Outros”. Esse ponto foi registrado como melhoria futura do protótipo.

## Privacidade e segurança

O protótipo segue os seguintes princípios:

- não solicita senha bancária;
- não solicita código de segurança;
- não realiza pagamentos;
- não realiza transferências;
- não movimenta dinheiro;
- não oferece empréstimos;
- não recomenda investimentos específicos;
- sempre solicita confirmação antes de registrar um gasto;
- permite desativar o uso de notificações;
- utiliza apenas dados fictícios.

## Limitações do MVP

O protótipo não possui:

- integração bancária real;
- acesso real às notificações do celular;
- Open Finance;
- pagamentos;
- Pix;
- autenticação bancária;
- banco de dados real;
- agente conectado a uma IA em produção.

A chegada das notificações bancárias é apenas uma simulação visual.

## Evolução futura

Uma versão funcional poderá utilizar:

- Lovable para a interface;
- aplicativo Android para leitura autorizada de notificações;
- n8n para automação;
- Ollama para interpretação local;
- PostgreSQL para armazenamento;
- webhook para receber as notificações;
- API para conectar o aplicativo ao n8n.

Fluxo conceitual:

```text
Notificação bancária
        ↓
Aplicativo Android autorizado
        ↓
Webhook do n8n
        ↓
Ollama interpreta a movimentação
        ↓
Usuário confirma no FinanChat
        ↓
PostgreSQL salva os dados
        ↓
Painel financeiro é atualizado


## 📱 Telas do FinanChat

As principais telas do projeto estão reunidas no arquivo abaixo:

[📄 Visualizar telas do FinanChat](./Imagens_FinanChat.pdf)
