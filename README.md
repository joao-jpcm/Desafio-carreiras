
# Banco digital

API REST de um banco digital que permite que os usuários realizem operações bancárias através de solicitações HTTP. Essa API pode ser utilizada para:

-   Criar uma conta
-   Listar contas
-   Atualizar os dados do usuário
-   Excluir conta
-   Depósitar
-   Sacar
-   Transferir 
-   Consultar saldo
-   Emitir extrato

Os endpoints dessa API podem ser protegidos por autenticação e autorização, garantindo a segurança das transações.

Esta API foi desenvolvida para conclusão do desafio do módulo 02 do curso de desnvolvimento de software fullstack da cubos academy

## Endpoints

#### Criar uma nova conta bancária

```http
  POST /contas
```

**Requisição do body**



#### Listar contas

```http
  get /contas?senha_banco=Cubos123Bank
```
essa "senha_banco" pode ser alterada para uma de sua escolha

**Requisição do body**


#### Atualizar dados da conta

```http
 PUT/contas/:numeroConta/usuario
```

**Requisição do body**


#### Excluir conta  

```http
  DELETE /contas/:numeroConta
```

**Requisição do body**


#### Depósitar

```http
  POST /transacoes/depositar
```

**Requisição do body**


#### Sacar

```http
  POST /transacoes/sacar
```

**Requisição do body**

#### Transferir

```http
  POST /transacoes/transferir
```

**Requisição do body**

#### Consultar saldo

```http
  GET /contas/saldo?numero_conta=123&senha=123
```

**Requisição do body**

#### Extrato da conta

```http
  GET /contas/extrato?numero_conta=123&senha=123
```

**Requisição do body**




