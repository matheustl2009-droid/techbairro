# Manual de uso da TechBairro

![Tela principal](img/tela_principal.png)

## A tela principal
A janela principal da TechBairro apresenta os campos de preenchimento para os dados dos moradores, o contador de cadastros ativos no rodapé, e os botões de ação: **Salvar**, **Consultar**, **Salvar edição**, **Excluir** e **Limpar**. Na parte inferior, uma área de mensagens exibe o feedback visual das operações realizadas.

## Cadastrar um cliente
1. Clique com o mouse no campo **Nome** e digite o nome completo do morador.
2. Clique no campo **Telefone** e informe o número com DDD.
3. Clique no campo **E-mail** e insira o correio eletrónico válido.
4. Clique no campo **Endereço** e preencha a morada completa.
5. Clique no botão **Salvar** para salvar os dados na base de dados local.

## Consultar os clientes cadastrados
1. Digite o nome do morador que deseja procurar no campo de pesquisa ou clique no botão **Consultar**.
2. Visualize as informações detalhadas que aparecem na lista de resultados do ecrã.
4.
## Alterar os dados de um cliente
1. Localize o cliente desejado através da consulta.
2. Selecione o registo correspondente na lista de moradores.
3. Modifique as informações necessárias diretamente nos campos de texto.
4. Clique no botão **Salvar edição** para atualizar os dados gravados.

## Excluir um cliente
1. Encontre e selecione o morador que deseja remover na lista de clientes.
2. Clique no botão **Excluir**.
3. Confirme a exclusão na mensagem de aviso que aparecerá no ecrã.

## Regras de preenchimento

| Campo | Obrigatório? | Regra |
|---|---|---|
| Nome | Sim | Deve conter pelo menos o nome e apelido, sem caracteres especiais inválidos. |
| Telefone | Sim | Formato numérico com DDD, preenchido sem letras. |
| E-mail | Sim | Deve incluir o caractere `@` e um domínio válido (ex: `.com`). |
| Endereço | Sim | Informar rua, número e bairro para localização precisa. |

## Mensagens do sistema

| Mensagem | O que significa | O que fazer |
|---|---|---|
| `Cliente cadastrado com sucesso!` | O registo foi gravado corretamente na base de dados. | Nenhuma ação necessária; os dados já constam no sistema. |
| `Preencha todos os campos obrigatórios!` | Existe algum campo em branco durante a tentativa de submissão. | Verifique os campos Nome, Telefone, E-mail e Endereço e preencha-os. |
| `Erro: E-mail inválido.` | O formato do endereço de correio eletrónico está incorreto. | Corrija o texto adicionando o símbolo `@` e o domínio correspondente. |
| `Registo não encontrado.` | A pesquisa efetuada não retornou nenhum morador correspondente. | Confirme a ortografia do nome procurado e tente novamente. |
| `Tem certeza que deseja excluir este registo?` | Janela de confirmação preventiva antes de apagar dados. | Clique em "Sim" se tiver certeza, ou "Não" para cancelar a operação. |
| `Banco em uso: techbairro.db` | Aviso impresso no terminal indicando a conexão ativa com a base de dados. | Apenas confirme que o sistema está pronto para uso na secretaria. |

## Dúvidas frequentes

* **O que fazer se o programa fechar sozinho ou der erro ao abrir?**  
  Certifique-se de que tem o Python instalado corretamente e que está a executar o comando a partir da pasta principal do projeto.

* **Os dados apagados por engano podem ser recuperados?**  
  Não diretamente pelo sistema. A recuperação exige a restauração da última cópia de segurança (*backup*) realizada do ficheiro `techbairro.db`.

* **Posso usar o sistema em mais de um computador ao mesmo tempo com os mesmos dados?**  
  Como o banco de dados é local (SQLite num único ficheiro), o sistema foi dimensionado para computadores individuais na secretaria, exigindo cópias manuais caso queira sincronizar dados entre máquinas diferentes.