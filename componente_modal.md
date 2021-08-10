
## Front-end | Módulo de Importação de valores - Listagem de tabela de franquias

:warning: **Resumo:** As telas fazem parte do fluxo de listagem/importação dos valores de franquia dos planos, esses valores são divididos em 3,para o estado do RJ,SP e demais estados. Os valores são contabilizados pela operadora de forma que o parceira atinja a meta estipulada.

:warning: **Proposta:** Após o usuário ter importado a tabela com sucesso ele é redirecionado para a tela de listagem, ou quando o usuario precisa consultar a lista de tabelas importadas. 

:bulb: **Caminho sugestivo:** `Cadastro -> Importação de Valores ->` `Cadastrar nova tabela` | `Ver todos`.


---
### :pushpin: Descrição
- Usuário acessa o módulo de importação de valores e seleciona a opção de ver todos ou após realizar um cadastro de tabela ele é redirecionado para a listagem.
#####  Tela de Listagem
- Usuário acessa a listagem de tabela de franquias, para consultar as informações sobre tabelas importadas.
- O sistema deve retornar um campo de busca por nome de usuario, por tipo de tabela ou estado.
- Os dados listados são (Nº, data de vigência, nome do usuario, tipo de tabela, e uma visualização de tabela), ai clicar no campo de ver tabela o usuario é redirecionado para a tela com detalhes sobre a importação da tabela.
#####  Tela de detalhes das tabelas de importação
- Ao  clicar em ver tabela o usuario é direcinado para outra tela onde terá informações e poderá fazer o download da tabela de franquias. 
- O sistema deve retornar os dados listados (data de vigência, nome do usuario, tipo de tabela, e UF destinada) além do arquivo importado e disponivel para download e um botão voltar caso o usuario queira retornar a listagem.
---

#### :rocket: Condições adicionais para a tela

- Possuir paginação.
- Versão mobile deve manter a consistência de espaçamento, deixando os itens em forma de blocos.
- Quantidade mínima de itens na tela 10+ itens.
- Possuir hover nos itens da lista.

#### :art:  Link do Figma com as telas

[Link do figma](https://www.figma.com/file/5Dc5FsbNBRMIOIm5BZHOia/Cadastro-de-valores-de-franquias-no-Gerencial?node-id=1325%3A11459)

Quaisquer dúvidas, estou a disposição.
