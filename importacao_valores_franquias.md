## Front-end | Módulo de Importação de valores - Importar tabela de franquias

:warning: **Resumo:** As telas fazem parte do fluxo de listagem/importação dos valores de franquia dos planos, esses valores são divididos em 3,para o estado do RJ,SP e demais estados. Os valores são contabilizados pela operadora de forma que o parceira atinja a meta estipulada.

:warning: **Proposta:** O usuário carrega o arquivo .csv, seleciona a data de vigência que será atual ou futura, o tipo da tabela **valor de franquia ou valor de referência"**, um ou mais UF’s,e realiza a importação. Após ser importado com sucesso o usuario deverá ser redirecionado para a tela de listagem.

:bulb: **Caminho sugestivo:** `Cadastro -> Importação de Valores ->` `Cadastrar nova tabela` | `Ver todos`.


---
### :pushpin: Descrição
- Usuário acessa o módulo de importação de valores e seleciona a opção de cadastrar nova tabela.
#####  Realizar Importação
- O sistema deve retornar um campo de upload de arquivos,um campo de data de vigência,um campo do tipo radio com as opções valor de franquia e valor de referência, campos de checkboxes com as UF's,um botão para baixar o modelo de importação e um botão para cadastrar.
- O usuário inicia o processo de importação adicionando um arquivo com a extensão .csv.
- No caso do arquivo inserido ter a *extensão diferente* do solicitado pelo sistema, é exibido uma mensagem de feedback ao usuário (Ex: Extensão não permitida)
- O usuario escolhe a data de vigência atual ou futura. Não poderá colocar data retroativa e deverá ser exibido um alerta informando o erro.
- O usuario deverá escolher o tipo da tabela **valor de franquia ou valor de referência"**
- O usuario deverá selecionar a UF desejada, pelo menos uma. Caso não selecionar não poderá prosseguir com a importação e deverá ser exibido uma mensagem de feedback ao usuário (Ex: selecione a UF desejada)
- Após todos os campos serem preenchidos corretamente deverá ser exibido ao usuario um feedback cadastro realizado com sucesso.
- Caso o usuario tente prosseguir sem importar nada ou preencher campos deve ser exibidos mensagens de feedback para que o mesmo selecione para cadastrar.
---

#### :rocket: Condições adicionais para a tela

- Validações correspondentes aos campos de entrada.
- Versão mobile deve manter a consistência de espaçamento, deixando os itens em forma de blocos.

#### :art:  Link do Figma com as telas

[Link do figma](https://www.figma.com/file/5Dc5FsbNBRMIOIm5BZHOia/Cadastro-de-valores-de-franquias-no-Gerencial?node-id=1325%3A11459)

Quaisquer dúvidas, estou a disposição.
