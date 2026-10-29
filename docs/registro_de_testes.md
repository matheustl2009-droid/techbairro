# Registro de testes da TechBairro
Versão testada: 3.3.2 · Data: 26/10/2026 · Responsável: Matheus Tavares de Lima
Sistema operacional e versão do Python: Windows 11 e Python 3.12.3
| ID | Requisito | Passos e dados | Esperado | Obtido | Status |
|---|---|---|---|---|---|
| CT01 | RF01 | Cadastrar um cliente com todos os campos certos | Cliente "cliente" Salvo com sucesso!| Cliente "cliente" Salvo com sucesso! | Passou|
| CT02 | RF01 | Salvar com Nome e Endereço vazios | Preencha o(s) campo(s):Nome, Endereço | Preencha o(s) campo(s):Nome, Endereço | Passou |
| CT03 | RF02 | Telefone 61 9999 0000 (com espaços) | Telefone inválido: use somente números |Telefone inválido: use somente números  | Passou |
| CT04 | RF03 | E-mail ana@email (sem ponto) | Email inválido: use o formato nome@dominio.com| Email inválido: use o formato nome@dominio.com | Passou |
| CT05 | RF05 | Editar um cliente, trocar o telefone e salvar | Cliente "cliente" atualizado com sucesso! | Cliente "cliente" atualizado com sucesso! | Passou |
| CT06 | RF06 | Excluir um cliente: responder Não, depois Sim | Cliente "cliente" excluído com sucesso | Cliente "cliente" excluído com sucesso  | Passou |
## Testes automáticos
Saída do `python testar_validacao.py`: 
OK teste_cliente_valido
OK teste_endereco_vazio
OK teste_telefone_com_letras
OK teste_email_sem_ponto
OK teste_nome_e_telefone_vazios
OK teste_email_sem_usuario
Todos os testes passaram.
## Defeitos encontrados
Nenhum (o que falhou, como foi corrigido e em qual commit; ou "nenhum")
