# Front-end | Módulo de Importação de margens - Importar tabela

## Fluxo do processo de importação de margens da operadora

:warning: **Resumo:** As telas fazem parte do fluxo de importação de margens, onde será realizada a importação de um arquivo pelo usuário com acesso ao modulo,automatizando um processo que hoje é realizado manualmente.


**Caso de uso**: Importação de arquivo para cadastro de margens.

**Pré-condição**: Atualmente contemplará apenas os módulo de importação de margens dentro do módulo de importações.

:bulb: **Caminho sugestivo:** `Importações -> Importação de margens ->` `Importar margens` | `Ver todas`.

### :pushpin: Descrição

#### Importar Margens

- Usuário acessa o módulo de importação de margers e seleciona a opção de importar.
---
##### Passo 1 - Realizar Importação
- Sistema deve retornar um campo de upload de arquivos e um botão para baixar o modelo de importação.
- O usuario inicia o processo de importação adicionando um arquivo com a extensão solicitada (extensão do arquivo a validar)
- No caso do arquivo inserido ter a *extensão diferente* do solicitado pelo sistema, é exibido uma mensagem de feedback ao usuario (Ex: Extensão não permitda)
- No caso do arquivo inserido ter a extensão solicitada pelo sistema o usuario pode avançar.
- Usuário clica em avançar.
- No caso do arquivo inserido ter o formato válido ele será direcionado ao **Passo 2**
- No caso do arquivo inserido *não ter o formato válido*, é exibido uma mensagem de feedback ao usuario (Ex:Arquivo em formato inválido) e o arquivo no campo é removido. 
---
##### Passo 2 - Dados da Importação
- O sistema deve retornar as informações referentes aos dados inseridos pelo usuário.
- Os dados são exibidos ao usuario em forma de tabelas com rolagem vertical dependendo da quantidade de dados.
- Os botões de "voltar" ao **Passo 1** e "salvar importação" ficam disponíveis ao usuario.
- Usuário pressiona botão "salvar importação" ele será direcionado ao **Passo 3**
---
##### Passo 3 - Concluído
- O Sistema retorna as informações de margens em forma de tabela e retorna o arquivo importado
- O botão "voltar" ao **Passo 2** fica disponível ao usuario
- No caso o usuario não clicar no botão "voltar" é exibido uma mensagem de feedback com a mensagem de sucesso e entao o usuário é redirecionado a listagem


#### Jobs Stories

**Quando** o usuario inserir um arquivo vazio
**Eu quero** que o sistema exiba uma mensagem de feedback
**Para que** ele possa selecionar um arquivo.

**Quando** o usuario inserir um arquivo de extensão inválida ou formato inválido
**Eu quero** que o sistema exiba uma mensagem de feedback
**Para que** ele possa selecionar um novo arquivo correspondende ao que o sistema está solicitando.

**Quando** o usuario for concluindo as etapas
**Eu quero** que o sistema sinalize visualmente 
**Para que** o usuario tenha melhor controle das etapas já realizadas.

#### :rocket: Condições adicionar para a tela

- Possuir hover nos itens da lista
- Validações correspondentes aos campos de entrada.
- Versão mobile deve manter a consistencia de espaçamento, deixando os itens em forma de blocos.

#### Itens adicionais

Adicionar Google Analitycs ao módulo, para gerarmos dados/informações de uso e realizarmos acompanhamento de sucesso do mesmo.
Adicionar captura/tracking de compartamento e eventos do Google Analitycs no módulo.

#### :art:  Link do Figma com as telas

[Link do figma](https://www.figma.com/file/bIbPVxbgvhOqqQ3iyn5RK4TN/DV-2482---Criar-menu-de-importa%C3%A7%C3%A3o-de-margens-no-geretim?node-id=81%3A591)

_Quaisquer dúvidas, me chame no slack com as dúvidas referentes ao card._
