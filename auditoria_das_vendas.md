# Front-end | Módulo de ______________ - Auditoria das Vendas

## Fluxo do processo de Auditoria das Vendas

:warning: **Resumo:** As telas fazem parte do fluxo de auditar as vendas e os status da fidelização de todos os planos e aparelhos na gestão documental. 


**Caso de uso**: Listagem de todos os tipos de venda de aparelho e/ou serviço da TIM.

**Pré-condição**: Essa tela faz parte do fluxo de gestão documental, onde são realizadas as audições das vendas e dos status da fidelização de planos e aparelhos.

:bulb: **Caminho sugestivo:** `Venda -> Pós-venda -> Gestão Documental ->` `Auditoria das Vendas`.

### :pushpin: Descrição

#### Importar Margens

- Usuário acessa o módulo de importação de margens e seleciona a opção de importar.
---
##### Passo 1 - Realizar Importação
- O sistema deve retornar um campo de upload de arquivos e um botão para baixar o modelo de importação.
- O usuário inicia o processo de importação adicionando um arquivo com a extensão solicitada (extensão do arquivo a validar)
- No caso do arquivo inserido ter a *extensão diferente* do solicitado pelo sistema, é exibido uma mensagem de feedback ao usuário (Ex: Extensão não permitida)
- No caso do arquivo inserido ter a extensão solicitada pelo sistema o usuário pode avançar.
- Usuário clica em avançar.
- No caso do arquivo inserido ter o formato válido ele será direcionado ao **Passo 2**
- No caso do arquivo inserido *não ter o formato válido*, é exibido uma mensagem de feedback ao usuário (Ex:Arquivo em formato inválido) e o arquivo no campo é removido. 
---
##### Passo 2 - Dados da Importação
- O sistema deve retornar as informações referentes aos dados inseridos pelo usuário.
- Os dados são exibidos ao usuário em forma de tabelas com rolagem vertical dependendo da quantidade de dados.
- Os botões de "voltar" ao **Passo 1** e "salvar importação" ficam disponíveis ao usuário.
- Usuário pressiona botão "salvar importação" ele será direcionado ao **Passo 3**
---
##### Passo 3 - Concluído
- O Sistema retorna as informações de margens em forma de tabela e retorna o arquivo importado
- O botão "voltar" ao **Passo 2** fica disponível ao usuário
- No caso o usuário não clicar no botão "voltar" é exibido uma mensagem de feedback com a mensagem de sucesso e então o usuário é redirecionado a listagem


#### Jobs Stories

**Quando** o usuário inserir um arquivo vazio
**Eu quero** que o sistema exiba uma mensagem de feedback
**Para que** ele possa selecionar um arquivo.

**Quando** o usuário inserir um arquivo de extensão inválida ou formato inválido
**Eu quero** que o sistema exiba uma mensagem de feedback
**Para que** ele possa selecionar um novo arquivo correspondente ao que o sistema está solicitando.

**Quando** o usuário for concluindo as etapas
**Eu quero** que o sistema sinaliza visualmente 
**Para que** o usuário tenha melhor controle das etapas já realizadas.

#### :rocket: Condições adicionais para a tela

- Possuir hover nos itens da lista
- Validações correspondentes aos campos de entrada.
- Versão mobile deve manter a consistência de espaçamento, deixando os itens em forma de blocos.

#### Itens adicionais

Adicionar Google Analytics ao módulo, para gerarmos dados/informações de uso e realizarmos acompanhamento de sucesso do mesmo.
Adicionar captura/tracking de comportamento e eventos do Google Analytics no módulo.

#### :art:  Link do Figma com as telas

[Link do figma](https://www.figma.com/file/bIbPVxbgvhOqqQ3iyn5RK4TN/DV-2482---Criar-menu-de-importa%C3%A7%C3%A3o-de-margens-no-geretim?node-id=81%3A591)

Quaisquer dúvidas, me chame no slack com as dúvidas referentes ao card.
