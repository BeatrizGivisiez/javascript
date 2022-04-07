# JavaScrit na prática!

- [1 - Funções](#funcoes)
- [2 - Map](#map)
- [3 - Set](#set)

## <a name="funcoes"></a> 1 - Funções
É um conjuto de instruções que executa uma tarefa/atividade.

### Sua declaração
A *declaração/definição* da função consiste no uso da palavra reservada/chave `function()`.

* Nome da função;
* Lista de argumentos para a função, entre parênteses e separados por vírgulas;
* Declarações JavaScript que definem a função, entre chaves {}, O que deve ser feito.
```javascript
function nomeDaFuncao(argumento){
    return argumento * argumento;
}
```

* A função `nomeDaFuncao` recebe um argumento chamado `argumento` entre chave. `nomeDaFuncao(argumento)`;
* A função consiste em uma instrução que indica para retornar o argumento vezes(*) o argumento, isto é: argumento multiplicado por si mesmo;
* A declaração `return` especifica o valor retornado pela função.
```javascript
    return argumento * argumento;
}
```

## <a name="map"></a> 2 - Map - Coleções Chaveadas
## MAP:
### Estrutura: 
const myMap = new Map()

### Caracteristicas: 
- Uma coleção de arrays no formato [chave, valor];
- Pode iterado por um loop for...of

### Argumentos:
clear: clear()
constructor: Map()
delete: delete()
entries: entries()
forEach: forEach()
get: funcao ()
has: has()
keys: keys()
set: ()
values: values()

### Métodos:
- Adicionar, consultar(ler) e deletar.

const myMap = new Map(chave, valor)
1ºChave: apple , 2ºValor: fruit

```javascript
set = adicionar
myMap.set('apple', 'fruit');
// Map(1) {"apple" => "fruit"}
myMap.get("apple");
// "fruit"
myMap.delete("apple");
// true
myMap.get("apple");
// undefined

### Qual a diferença entre Map vs Objeto, já que ambos contém chave e valor?
- Maps podem ter chaves de qualquer tipo;
- Maps possuem a propriedade length;
- Maps são mais fáceis de iterar;
- Maps utilizamos quando o valor das chaves é desconhecido;
- Os valores tem o mesmo tipo.

____
## <a name="set"></a> 3 - Set - Coleções Chaveadas
### Estrutura: 
const myArray = [1, 1, 2, 2, 3, 4, 5, 6, 7, 8, 2, 1]
const mySet = new Set(myArray)

Caracteristicas:
- Sets são estruturas que armazenam apenas "valores únicos".

Métodos:
- Adicionar, consultar(ler) e deletar.

```javascript
const mySet = new Set();
mySet.add(1);
mySet.add(5);
mySet.has(1);
// true
mySet.has(3);
// false
mySet.delete(5);
```

Qual a diferença entre Set vs Array, já que ambos contém chave e valor?
- Set possui valores únicos;
- Em vez da propriedade length, consulta-se o número de registros pela propriedade size.
- Não possui os métodos map, filter, reduce etc.
