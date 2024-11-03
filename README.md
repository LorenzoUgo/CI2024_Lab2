# CI2024_Lab2
_DEADLINE: **Sunday, November 3 @ 23:59 UTC**_
## Travel SalesMan Problem (TSP)
Our goal is to find a solution of TSP istances using both a fast but approximate algorithm and a slower but more accurate one.

I will evaluate the goodness of a solution considering final cost and number of steps.

<table>
  <tr>
    <td>

| Instance | Cities |
|----------|--------|
| Vanuatu  | 8      |
| Italy    | 46     |
| Russia   | 167    |
| Usa      | 326    |
| China    | 726    |
   </td>
   <td>
        
    Each cities is represented with geo-coordinates (lat, lon).
        
    For each pair of cities, we can compute their distance. So, the istance can be represented by with a fully connected graph.
   </td>
  </tr>
</table>

### How do I define "_Distance_" ?
I compute cities _distance_ with a geografic interpretation.

The _distance_ then become the value of the edge between two cities (nodes).


## Greedy Solution


|  Instance  |  Cities  | Final Cost (km) | Num Steps |
|:----------:|:--------:|:---------------:|:---------:|
| Vanuatu    | 8        | 1480.44         | 1         |
| Italy      | 46       | 4586.63         | 1         |
| Russia     | 167      | 41961.93        | 1         |
| Usa        | 326      | 46730.14        | 1         |
| China      | 726      | 63175.41        | 1         |

## Genetic Algorithm

My GA combine different techniques of parent selection, mutation and crossover. At the end of each generation, survives the most promising individuals: the ones with the better path.

>**Crossover**
>- _Inver Over_: 
>
>- _Partially_Mapped_Crossover_: 
>

>**Parent Selection**
>- _Roulette wheel_: 
>
>- _Roulette wheel fitness based_: 
>
>- _Best parent_: 
>

>**Mutation**
>- _Macro mutation_: 
>
>- _Insert mutation_: 
>
>- _Inversion mutation_: 
>

Num. steps =  [_number of path computed_] = starting_population + (num_offspring*num_generations)

|  Instance  |  Cities  | Final Cost (km) | Num Steps |
|:----------:|:--------:|:---------------:|:---------:|
| Vanuatu    | 8        |  1345.54        | 520       |
| Italy      | 46       |  6449.58        |  6040     |
| Russia     | 167      |  75497.79       |  40050    |
| Usa        | 326      |  83389, 51      | 300050    |
| China      | 726      |       |  4500100     |