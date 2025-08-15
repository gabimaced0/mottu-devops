# Mottu Backend - DevOps Tools & Cloud Computing

Repositório exclusivo para a entrega da Sprint 3 da disciplina **DevOps Tools & Cloud Computing**.

Integrantes
- Fernando Henrique Vilela Aguiar — RM557525
- Gabrielly Campos Macedo — RM558962
- Rafael Macoto Magalhães — RM554992

Este backend Java permite gerenciar motos com integração ao **Azure SQL Database** e deploy em **Azure Container Instance (ACI)**, com imagem armazenada no **Azure Container Registry (ACR)**.

---

## Descrição da Solução

Aplicação Java com API REST que realiza CRUD completo sobre a entidade **Moto**, permitindo cadastrar, listar, editar e excluir motos da base de dados. O backend foi containerizado e publicado no Azure.

---

## Benefícios para o Negócio

- Automatiza o controle de motos da empresa
- Centraliza informações em banco na nuvem
- Garante escalabilidade e portabilidade com Docker + Azure
- Permite deploy rápido sem infraestrutura complexa (via ACI)

---

## Banco de Dados em Nuvem (Azure SQL)

- Banco: `dbmottu`
- Servidor: `rm558962.database.windows.net`
- Usuário: `mottuuser`
- Conexão: configurada via variável de ambiente `SPRING_DATASOURCE_URL`
- Conexão JDBC (exemplo):

```properties
jdbc:sqlserver://rm558962.database.windows.net:1433;database=dbmottu;user=mottuuser@rm558962;password=SENHA_AQUI;encrypt=true;trustServerCertificate=false;hostNameInCertificate=*.database.windows.net;loginTimeout=30;


