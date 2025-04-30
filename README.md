# SG - Yia ( Sistema de gestão - Yia)

## Descrição

O **SG - Yia** é uma solução de gestão e faturamento para PMEs e lojas que vendem produtos físicos. Ele automatiza e simplifica controle estoque, vendas, emissão de faturas, gestão de funcionários e controle de usuários. O sistema de tem suporte a **multiempresa (multi-tentat)** baseda em `empresa_id`, de momento usa autenticação padrão do Laravel através de sessões.

---
## Funcionalidades

- Cadastro de empresa, de produtos(juntamente com o fornecedor de momento), clientes, funcionários e usuários
- Controle de estoque
- Emissão de faturas e recibos
- Multiempresa (multi-tenant) por  `empresa_id` via Eloquent
- Autenticação com sessões padrão do Laravel

---
## Tecnologias

- **Back-end:** Laravel 10
- **Front-end:** Blade, Vite, TailwindCSS, Bootstrap e Axios.
- **Banco de dados:** MySQL
- **Tenancy:**  `empresa_id` através de filtros directos nas consultas ao banco

---
## Instalação local

- **Requisitos**

- **PHP:** Versão ^8.2
- **Node.js:** Versão >=16
- **Composer:** Instalado
- **npm:**Instalado

- **Passos**

- 1.Clone o repositório:
```bash
git clone <url>
cd sg-ya
```
- 2.Instale as dependências do back-end:
```bash
composer install
```
- 3.Instale as dependências do front-end:
```bash
npm install
```
- 4.Configure o arquivo .env: copie o arquivo .env.example para .env
```bash
cp .env.example .env
```
- 5.Gere a chave da aplicação:
```bash
php artisan key:generate
```
- 6.Execute as migrações:
```bash
php artisan migrate
```
- 7.Inicie o servidor de desenvolvimento: retira o elemenot **/nova** dos links do dashboard para que não ocorra erro pela rota não ser encotrada

```bash
php artisan server
```
```bash
npm run dev
```

---
## Como contribuir
Não disponivél para a contribuição de momento

---
## Documentação
A documentação completa está disponível nos arquivos dentro da pasta /docs

- **Configuração do Ambiente**
- **Tency com empresa_id**
- **Autenticação**
- **Módulo do Sistema**

---
## Licença
MIT