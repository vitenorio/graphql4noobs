## Conceito de Queries e Mutations

As Queries são usadas para solicitar dados da sua api, o que seria equivalente ao metodo GET no http. Já as Mutations são utilizadas para criar, atualizar e excluir dados.

## Campos

O GraphQL permite pedi para a api apenas os campos que serão utilizados, isso é uma vantagem para diminuir o consumo de dados.

| ` 
{
  usuário {
    nome
  }
}
` 
| 