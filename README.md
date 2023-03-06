
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

![criar conta](https://user-images.githubusercontent.com/111611674/223001862-b6ed153d-0db7-4341-a9f6-cbc41f9d5b1d.jpg)

**Resposta**

sem resposta, apenas status code

#### Listar contas

```http
  get /contas?senha_banco=Cubos123Bank
```
**Requisição do body**

essa "senha_banco" pode ser alterada para uma de sua escolha

**Sem resquisição no body**

**Resposta**

![res listar contas](https://user-images.githubusercontent.com/111611674/223001970-af4c0044-8a68-420e-9931-c605f4a5c03b.jpg)

#### Atualizar dados da conta

```http
 PUT/contas/:numeroConta/usuario
```

**Sem requisição no body**

**Resposta**

![res atualizar](https://user-images.githubusercontent.com/111611674/223002184-2897d2b8-62f0-428a-aeaf-413c4c6e48ef.jpg)


#### Excluir conta  

```http
  DELETE /contas/:numeroConta
```

**Sem requisição no body, apenas retorno do status code**


#### Depósitar

```http
  POST /transacoes/depositar
```

**Requisição do body**

![req depositar](https://user-images.githubusercontent.com/111611674/223002446-7a25453b-ccc1-4271-abf3-cf0f57ff2e9e.jpg)

**Resposta**

sem resposta, apenas status code

#### Sacar

```http
  POST /transacoes/sacar
```

**Requisição do body**

![req sacar](https://user-images.githubusercontent.com/111611674/223002475-447fd490-3047-4fe1-9665-c8b39c205975.jpg)

**Resposta**

sem resposta, apenas status code

#### Transferir

```http
  POST /transacoes/transferir
```

**Requisição do body**

![req transferir](https://user-images.githubusercontent.com/111611674/223002489-8c1f8a69-bc6d-482a-b52d-c4f3c6d97c88.jpg)

**Resposta**

sem resposta, apenas status code

#### Consultar saldo

```http
  GET /contas/saldo?numero_conta=123&senha=123
```

**Sem requisição no body**

**Resposta**

![res saldo](https://user-images.githubusercontent.com/111611674/223002569-c25ef731-b9b5-45ff-8ff2-58a0a4a6013c.jpg)


#### Extrato da conta

```http
  GET /contas/extrato?numero_conta=123&senha=123
```

**Sem requisição no body**

**Resposta**

![res extratos](https://user-images.githubusercontent.com/111611674/223002583-b0dd9eaa-17e4-4ec1-9c90-015497247854.jpg)





