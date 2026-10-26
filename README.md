# TechBairro
Sistema de cadastro e gestão de moradores desenvolvido para informatizar os atendimentos da associação de moradores do bairro. 
(uma ou duas frases: o que o sistema faz e para quem)
**Versão atual:** 3.3.1 · Histórico de mudanças no [CHANGELOG](CHANGELOG.md)
## Funcionalidades
- Cadastro de novos moradores/clientes.
- Consulta de moradores cadastrados.
- Alteração de dados cadastrais.
- Exclusão de registros.
## Requisitos para execução
| Item | Requisito |
|---|---|
| Sistema operacional | Windows 10 / 11, Linux ou macOS|
| Python |Versão 3.10 ou superior (versão testada: 3.12.3) |
| Tkinter | Nativo da biblioteca padrão do Python |
| Bibliotecas externas |Nenhuma (projeto sem dependências externas) |
| Internet |Opcional (apenas para download inicial do repositório)|
## Instalação
1. Na página principal do repositório no GitHub, clique no botão verde Code.

2. Selecione Download ZIP.

3. Extraia o arquivo ZIP compactado em uma pasta no seu computador.

4. Abra o terminal (ou prompt de comando), entre na pasta extraída e execute:
    python techbairro.py

## Configuração do banco de dados
- Onde fica: O banco de dados fica guardado num único ficheiro local chamado techbairro.db, criado na mesma pasta raiz onde o programa é executado.

- Quando é criado: O ficheiro e as tabelas são gerados automaticamente na primeira vez que o sistema é iniciado, caso ainda não existam.

- Como saber qual banco está em uso: Através da mensagem impressora no terminal (Banco em uso: techbairro.db).

- Por que ele não vem no repositório: Para cumprir as normas de privacidade e proteção de dados da LGPD (Lei Geral de Proteção de Dados), evitando expor dados reais de moradores na nuvem pública. O ficheiro está devidamente bloqueado pelo arquivo .gitignore.

- Como fazer uma cópia de segurança (backup): Basta copiar o ficheiro techbairro.db e guardá-lo periodicamente numa pasta segura ou suporte externo
## Como usar
- O passo a passo está no [Manual de uso](docs/manual_de_uso.md).
## Estrutura do projeto
- techbairro.py: Ficheiro principal que inicia a aplicação e gerencia as telas.

- requirements.txt: Lista informativa de dependências da biblioteca padrão.

- .gitignore: Configuração para ignorar ficheiros locais e o banco de dados.

- docs/manual_de_uso.md: Manual detalhado de utilização do sistema para a secretaria.

- docs/img/: Pasta reservada para os prints de tela da documentação.
## Autor
Matheus Tavares de Lima

Curso: Técnico em Desenvolvimento de Sistemas

Instituição: SENAC DF