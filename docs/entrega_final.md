# Entrega final da TechBairro
Aluno(a): Matheus Tavares de Lima · Versão entregue: v3.3.2
Por que esse número de versão: A versão 3.3.1 era a última estável e, como desde então foram adicionados apenas documentação e ajustes de arquivos de suporte sem alterar a lógica principal, soma-se 1 ao último número da versão.
| # | Item | Evidência |
|---|---|---|
| 1 | A aplicação funciona: os 6 casos de teste passaram | docs/registro_de_testes.md |
| 2 | A versão aparece na janela e é a mesma do CHANGELOG e do README | Sim |
| 3 | O pacote foi testado numa pasta limpa | Testado com dist/TechBairro-3.3.2.zip extraído|
| 4 | Tag e release publicadas, com o .zip anexado | https://github.com/matheustl2009-droid/techbairro/releases/tag/v3.3.2 (link da release) |
| 5 | O repositório não tem banco, __pycache__ nem dist | Verificado pelo .gitignore |
| 6 | O histórico tem commits com mensagens claras |https://github.com/matheustl2009-droid/techbairro/commits/main/ (link dos commits) |
| 7 | README, manual de uso e requirements.txt estão no repositório | Sim |
| 8 | A Issue "Teste do README" (Aula 26) está fechada | https://github.com/matheustl2009-droid/techbairro/issues/1 |
| 9 | O vídeo está publicado e o link abre sem pedir login | https://drive.google.com/file/d/1LuUTh44uwJiU1hNaK3AYGQmiPB4418Ge/view?usp=sharing (link do vídeo) |
## Roteiro do vídeo
| Bloco | Tempo | O que vou mostrar ou dizer |
|---|---|---|
| 1. Problema e solução | 30 s |  A associação de moradores da TechBairro precisava de um sistema simples e seguro para gerenciar cadastros de moradores e parceiros. A TechBairro 3.3.2 resolve isso com uma aplicação desktop rápida, persistência em SQLite e validações completas. |
| 2. Demonstração | 1 min 30 s | O caminho que vou seguir: cadastrar um novo cliente, consultar a lista, editar um dado, excluir um registro e demonstrar uma regra de validação (como telefone ou e-mail incorreto) sendo barrada pelo sistema. |
| 3. Como foi construída | 30 s | O projeto foi estruturado em Python com Tkinter para interface gráfica, banco SQLite, testes automatizados e controle de versão no GitHub, gerando um pacote .zip via script de release. |
| 4. Aprendizado | 30 s | Como melhoria futura para o projeto, eu implementaria a transição entre os campos de escrita utilizando as setas do teclado para facilitar a digitação rápida dos dados. |

## Perguntas

• Pergunta 1: por que o arquivo techbairro.db não está no GitHub?
Porque o banco de dados armazena dados locais e dinâmicos, sendo ignorado pelo .gitignore para que cada ambiente crie a sua própria base limpa na primeira execução.

• Pergunta 2: qual caso de teste (desta entrega ou das Aulas 15, 20 e 21) pegou um defeito de verdade? Qual era o defeito?
O teste CT04 (validação de e-mail sem ponto) identificou que a verificação inicial aceitava formatos incorretos. O erro foi corrigido ajustando a função de validação no código fonte.

• Pergunta 3: se o voluntário da associação tiver só o link do repositório, como ele instala e executa a TechBairro?
Ele deve acessar a aba de Releases do repositório no GitHub, baixar o arquivo .zip da versão mais recente, extraí-lo, abrir o terminal na pasta, instalar as dependências com `pip install -r requirements.txt` e executar `python techbairro.py`.

## Autoavaliação
O vídeo ficou direto e cobriu com clareza todas as funcionalidades do CRUD e as regras de validação dentro do limite de tempo. O que mudaria seria apenas a preparação prévia dos cliques para otimizar a navegação. O aprendizado mais marcante foi dominar o processo completo de empacotamento, versionamento e entrega de um software desktop pronto para o usuário final.
