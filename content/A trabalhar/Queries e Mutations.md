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

## Argumentos

No GraphQL, os campos e objetos podem ter seu próprio conjunto de argumentos, tornando o GraphQL um substituto completo para várias buscas de API.

```
{
  usuario(id: "100") {
    nome
    altura
  }
}
````

Retorno da api:
```
{
  "data": {
    "usuario": {
      "name": "Vitoria",
      "height": 1.65
    }
  }
}
```
