## Conceito de Queries e Mutations

As Queries são usadas para solicitar dados da sua api, o que seria equivalente ao metodo GET no http. Já as Mutations são utilizadas para criar, atualizar e excluir dados.

## Campos

O GraphQL permite solicitar apenas os campos que serão utilizados, isso é uma vantagem para diminuir o consumo de dados.

Nesse exemplo de Query, pedimos para a api só o campo nome:
```
{
  usuario {
    nome
  }
}
```

E a api retorna: 
```
{
  "data": {
    "usuario": {
      "nome": "Vitoria"
    }
  }
}
```
