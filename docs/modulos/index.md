# Módulos do sistema
Abaixo estão listados os principais módulos do sistema

**obs:** Antes de começar a usar o sistema é necessário ter uma empresa registrada, o sistema não vem com dados para serem populados
---
## Produos
- Cadastro com o fornecdor incluidio fora os dados do produto.
- Movimentação ao vender ou faturar
- Atualizçaõ dos dados do produto
- Filtragem por nome, fornecedor, codigo e categoria

---
## Clientes
- Cadastro com nome(obrigatório), telefone(obrigatório), morada, email, faixa etária e gênero
- Associado a empresa_id
- O cliente pode ser cadastro no momento da venda, caso o cliente não esteja registrado na base de dados o registro será feito automaticamente no momento da venda
- Os dados utilizados para chegar se estamos a tratar do mesmo cliente ou não é o nome e o telefone - incluindo a emrpesa_id para saber se a empresa conhece o cliente

---
## Vendas e Faturamento
- Criação de faturas com produtos, impostos e desontos
- Geração de recibo e fatura em pdf - são gerados do banco quando se precisa, podem ser impressos, salvos ou enviados
- filtro por cliene, status, codigo(id), venedor - para fatura
- Toda venda gera automaticamente uma fatura
- Toda vez que uma fatura é marcada como paga, é feita a atualização automática do estoque

---
## Funcionários
- Cadastro, edição  e remoção de funcionários
- O funcionário pode ser cadastrado como sendo usuário do sistema ou não

---
## Usuários
- Cadastro do usuário
- O usuário admin da empresa é registrado no momento do cadastro da empresa, os demais usuários são cadastrados pelo admin ou gerente
- Remoção do usuário

## Empresa
- Registro de empresa
- Antes de começar a usar o sistema precisa registrar uma empresa com os dados básicos, **dados fiscais(NIF) e endereço , dados do proprietário e o admim do sistema para aquela empresa** 