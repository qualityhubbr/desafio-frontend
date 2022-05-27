# Desafio Frontend QualityHub

Faça um fork deste repositório e comece a trabalhar no código!

## Objetivos

Utilizando os frameworks e bibliotecas de sua preferência crie uma visualização para os 151 pokémons utilizando a [Pokeapi](https://pokeapi.co/).

A visualização terá 2 principais blocos na vertical.

### Bloco de gráficos

Deverá ter um gráfico de pizza de acordo com número de pokemons de cada tipo. Utilizando o atributo do pokémon `types[].type.name`. Caso o pokemon tenha mais de um tipo, ele irá contar mais de uma vez no gráfico.

Deverá ter um gráfico de barras. Mostrando no eixo X a quantidade de habilidade, 1, 2, 3 ou 4, e no eixo Y a quantidade de pokemons com aquela quantidade de habilidades. Para ver a quantidade de habilidades, é só ver o tamanho do atributo do pokémon `abilites`.

Imagem com uma idéia de layout ilustrando os dois blocos.

![image](https://user-images.githubusercontent.com/308200/170794502-8ec88240-f69f-4db7-87da-46bc6df87bbf.png)


### Lista de pokémons

Deverá fazer uma lista utilizando o método de sua preferência (lista de cards, tabela, etc). Esta lista deverá conter:
* Nome do Pokémon `name`
* Quantidade de Habilidades `abilites.length`
* Tipos `types[].type.name`
* Sprite do Pokemon `sprites.frontDefault`


## Dica: Pegando os dados da API

Para buscar os dados, primeiro é necessário buscar todos os 151 pokémons, que são os pokémons clássicos da primeira geração. (https://pokeapi.co/api/v2/pokemon?limit=151)

Após buscar estes dados. Os pokémons estarão no atributo `results[]`.

Para buscar os dados individuis com todos os atributos listados dos pokémons, é só chamar a url contida em cada entrada de pokémon: `results[].url`
