
## Front-end | Componenização de modal

## O novo componente poderá ser reutilizado no processo de novos módulos e refatoração de antigos.Teremos ganhos na reutilização de trechos de código, no isolamento de contexto, na legibilidade do código, e na padronização do projeto.


:warning: **Resumo:** Esse modal faz parte do fluxo de transferencia, onde são realizadas os cadastros e listagem de transferencia.

**Pré-condição:** Atualmente contemplará apenas o módulo de transferencia.


---
### :pushpin: Descrição
- Sistema apresenta a visualização da mensagem de feedback em forma de modal para o usuario após ser realizada uma transferencia, trazendo a visualização de forma adaptativa ao conteúdo inserido
- Modal deve ser responsivo.
- Modal deve apresentar informações como scroll.
- Usuário deve poder clicar no botão concluir para fechar o modal.
- Usuário deve poder clicar no botão repetir para voltar a tela onde estava.


#####  Componente
- 
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
