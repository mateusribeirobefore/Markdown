# Componenização de botões

## O novo componente poderá ser reutilizado no processo de novos módulos e refatoração de antigos.Teremos ganhos na reutilização de trechos de código, no isolamento de contexto, na legibilidade do código, e na padronização do projeto.


As telas fazem parte do fluxo de devolução de venda, onde será realizada as devoluções de produtos e acessórios da loja.
Processo realizado pelos Vendedores ou BackOffice da loja.

**Caso de uso**: Listagem de contatos de vendas realizadas.

**Pré-condição**: Atualmente contemplará apenas os módulo de devolução da venda dentro do módulo de compra.

:bulb: **Caminho sugestivo:** `Venda -> Venda -> Devolução da venda ->` `Inserir registro` | `Ver todos`.

### :pushpin: Descrição

#### Inserir registro

- Usuário acessa o formulario de devolução.
- Sistema deve retornar as informações do formulário.
- Usuário pode iniciar uma devolução apartir dos dados pessoais [**Nome**, **CPF**] do cliente ou atravéz do [**Número da venda**] para dar inicio ao processo de devolução.
- Sistema deve retornar as informações referentes aos dados inseridis pelo usuário.
- No caso de inserido Nome e CPF do cliente, o sistema deve retornar as 3 ultimas vendas realizadas para o cliente informado.
- No caso de Número da venda, o sistema deve retornar pontualmente a venda.

- O Sistema retorna as informações da venda selecionada
- Usuário deve escolher 1 ou Todos, items da venda para a devolução.
- Usuário seleciona os itens desejados na listagem da venda especifica.
- Usuário pressiona o botão avançar.
- Sistema retorna um resumo dos itens selecionados para a devolução.
- Quando ouver acessórios a devolver, sistema deve permitir a inserção de quantidade pelo usuário.
- Sistema deve validar a quantidade de acessórios adicionado pelo usuário. O Valor deve ser **Maior/Igual(>=)** que 0 (Zero) e **Menor/Igual(>=)** que a quantidade de acessorios da venda.

- Usuário pressiona botão "Salvar devolução"
- Sistema valida informações e realiza o processo de salvar a devolução.
- Sistema retorna uma tela com botão para emitir nf-devolução.
- Sistema verifica todas as etapas preenchidas pelo usuário.

- Usuário pode emitir NF-devolução ou concluir o processo de devolução.
- Usuário deve clicar no botão "Concluir" para finalizar o processo de devolução da venda
- Sistema redireciona o usuário para a listagem de devoluções cadastradas no sistema.

- Usuário pode emitir NF-devolução ou concluir o processo de devolução.
- Usuário deve clicar no botão "Concluir" para finalizar o processo de devolução da venda.
- Sistema redireciona o usuário para a listagem de devoluções cadastradas no sistema.

#### 2. Visualizar todos

#### Jobs Stories

**Quando** as ativações forem realizadas
**Eu quero** ser informado da ativação e qual forma (Contole, Pós, Internet e pré-pago)
**Para que eu** tenha melhor controle do faturamento e metas, além de calcular o complemento da remuneração do vendedor.

**Quando** as devolução for realizadas.  
**Eu quero** poder realizar a emissão da Nota Fiscal de devolução.  
**Para que eu** tenha melhor controle das devoluções cadastradas, afim de evitar a não emissão da nota fiscal.

**Quando** acessar listagem de devoluções
**Eu quero** visualizar os registros de devolução da filia(Que tem acesso ou Todas), em orde da mais recente para a mais antiga.
**Para que eu** tenha melhor controle das devoluções realizadas.

**Quando** eu desejar realizar uma buscar personalizada das devoluções
**Eu quero** poder filtrar por (Nome/CPF do cliente, Filiais, Periodo - inicio e fim)
**Para que eu** possa seletizar a busca de acordo com a minha necessidade.

**Quando** estiver na listagem de devoluções
**Eu quero** poder inserir uma nova devolução
**Para que eu** não precise acessar o módulo do inicio, me permitindo utilizar um atalho para o cadastro de uma nova devolução.



**Quando** estiver na listagem de devoluções
**Eu quero** poder remover uma devolução
**Para que eu** possa remover um movimento que foi inserido de maneira errada.

**Quando** estiver na listagem de devoluções
**Eu quero** emitir uma nota fiscal de devolução de um registro de devolução que desejo.
**Para que eu** possa garantir que não será mais necessaria a edição de uma devolução e transmitir no periodo correto.

**Quando** estiver na listagem de devoluções
**Eu quero** editar um registro de devolução desejado
**Para que eu** realizar a alteração das informações que possam estar incorretas ou adicionar novos itens a devolver.

- Usuário pode clicar no botão de ações de cada item da lista.  
  - Sistema deve retornar um menu com as seguintes opções:
  - visualizar devolução
  - Emitir nf-devolução
  - Editar devolução
  - Remover devolução

#### :rocket: Condições adicionar para a tela

- Possuir paginação, quando houve mais que a quantidade minima de itens na tela 20+ itens.
- Possuir hover nos itens da lista
- Filtro de listagem de devoluções deve possuir mascara nos campos dos filtros.
- Remover um item da listagem, deve possuir um modal de confirmação para a exclusão.
- Menu de ações direcionar o usuário para outras partes do sistema referente ao menu clicado.
- Versão mobile deve manter a consistencia de espaçamento, deixando os itens em forma de blocos.

#### Itens adicionais

Adicionar Google Analitycs ao módulo, para gerarmos dados/informações de uso e realizarmos acompanhamento de sucesso do mesmo.
Adicionar captura/tracking de compartamento e eventos do Google Analitycs no módulo.

#### :art:  Link do Figma com as telas

[Link do figma](https://www.figma.com/file/JbRo6TtowHGUg1dL3v3pDt/DV-1787-Cria%C3%A7%C3%A3o-do-m%C3%B3dulo-de-Devolu%C3%A7%C3%A3o-de-Venda?node-id=146%3A693)

_Quaisquer dúvidas, me chame no slack com as dúvidas referentes ao card._
