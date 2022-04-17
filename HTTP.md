# Request and Responses

We will be working on Pokemon Search

## Creating index

Index is a collection of similar documents. Eg., Products, Pokemons, etc.

### Request

```
PUT pokedex?pretty
{
	"settings": {"number_of_shards": 1,"number_of_replicas": 0}
}
```

### Response

```
Status: 200

{
  "acknowledged" : true,
  "shards_acknowledged" : true,
  "index" : "pokedex"
}
```