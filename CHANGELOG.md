# Changelog da TechBairro

## Em desenvolvimento
### Adicionado
- Código publicado no GitHub, com histórico de versões.

## v3.3.1 (Aula 21) 

### Alterado
- O código monolítico do `techbairro` foi reorganizado em arquitetura de camadas.
- A classe `Cliente` foi movida para o novo módulo `cliente.py`.
- A comunicação com o banco de dados SQLite foi isolada no novo módulo `banco.py`.
- As regras de negócio de validação foram centralizadas na classe `ValidadorCliente` dentro do novo módulo `validacao.py`.

### Adicionado
- Criado o script de testes automatizados unitários `testar_validacao.py` para validar as regras de negócio de forma isolada, sem interface gráfica e sem mexer no banco de dados.

## v3.3.0 (Aula 20)

### Adicionado
- Modo de edição visível, com o botão alterando para “Salvar edição”.
- Edição de cliente por duplo clique na lista da Consulta.
- Proteção para impedir edição ou exclusão de linhas informativas.
- Mensagens específicas ao cancelar uma edição.

### Corrigido
- Edição e exclusão passam a usar o cliente correspondente à linha selecionada na tela.
- O sistema confere se o banco realmente atualizou ou removeu o cliente.
- Aviso quando o cliente já não existe mais no banco.
- Lista da Consulta atualizada após tentativas de exclusão de registros inexistentes.

## v3.2.1 (Aula 18)
### Alterado
- O número da versão passou a ficar v3.2.1
### Adicionado
- Script scripts/gerar_pacote.py, que monta um arquivo .zip e deixa fora o que não deve ser distribuido
- Arquivo COMO_EXECUTAR.txt, com a nova versão explica os requisitos, forma de execultar e os dados que vão ser 
apresentados


## v3.2.0 (Aula 16)

### Alterado
- O banco agora é aberto pelo caminho completo (os.path + _
_file__),
sempre na pasta do projeto, não importa de onde o programa seja executado.

### Adicionado
- Mensagem "Banco em uso" no terminal, mostrando qual arquivo de banco está sendo usado.

Atividade: Organizando e Versionando o Projeto TechBairro 3

## v3.1 (Aula 15)

### Corrigido
- Atualizar() com commit
- Verifica a validação
- Validação do e-mail
- Agora passa a recusar e-mails sem pontos depois do @
- Passando a mensagem de "formato inválido"


## v3.0 (Aula 14)

### Alterado
- O GerenciadorClientes deixou de guardar os clientes numa
- Lista em memória e passou a gravar no banco SQLite techbairro.db
- Tela foi atualizada para usar ids do banco em vez de índices de lista.
- Operações crud (adicionar, listar, atualizar, remover) agora persistem no banco.

### Adicionado
- Interface gráfica principal (cadastro) com formulário e botões de salvar, consultar e limpar.


## v2.0 (Aulas 11 e 12)

### Adicionado
- Implementação das classes de domínio e a tela de consulta com listagem e seleção de clientes.

## Antes da v2.0 (Aulas 5 a 10)
- Protótipos de telas, eventos e validações básicas do formulário (campos obrigatórios, navegação entre campos).