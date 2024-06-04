## Screening
Este repositório contém um teste simples que deve ser aplicado em caráter de "screening" para vagas de Node.js na ST-One.

### Teste 1

**Implemente uma classe para uma fila com prioridades**

Neste desafio você deverá criar uma fila com prioridade. Uma fila com prioridade é um tipo especial de fila onde itens adicionados possuem informações adicionais que especificam a sua prioridade. Isto pode ser simplesmente representado por um número inteiro. A prioridade de um item irá determinar a sequência na qual tiraremos itens da fila. Se um item possui uma prioridade maior, será removido da fila antes que os itens com menos prioridade, quanto maior a sua prioridade, antes será removido da fila.

Por exemplo, vamos imaginar que possuímos uma fila com os seguintes itens:

```json
[{"name":"Gato", "priority": 1}, {"name":"Cachorro", "priority": 4}, {"name":"Coelho", "priority": 2}, {"name":"Vaca", "priority": 3}]
```

Neste caso a prioridade é definida como um inteiro. Se colocarmos na fila o "Gato" com prioridade 1 (assumindo que números menores tem precedência na prioridade), então ele seria o primeiro a sair da fila.

Para o desenvolvimento, você deverá adicionar um método de adicionar itens na fila, remover itens da fila, retornar os itens da fila, mostrar a quantidade de itens na fila, um método de "front" para mostrar o elemento no início da fila e um método que retorne um booleano informando se a fila está vazia ou não.

O método de adição de itens na fila deve aceitar objetos conforme demonstrado acima, com propriedades de "name" e "priority".
Os métodos de remoção dos itens da fila e de "front" devem retornar apenas o "name" do item.

O desafio deve ser completado em uma sessão de screening com duração de 1h. Evite utilizar frameworks e bibliotecas, para minizar o tempo de setup e a complexididade.
Foque em implementar funcionalidades principais, evitando "features" desnecessárias.
Critérios da avaliação:

- **Funcionalidade**: O sistema consegue adicionar, excluir, imprimir itens de uma fila de maneira eficiênte?
- **Qualidade de código**: O código está bem estruturado, legível e manutenível? Boas práticas foram seguidas?
- **Documentação**: Métodos foram documentados e instruções para execução do código foram providênciadas?

Nota: A avaliação será focada na completa implementação e aderência aos requerimentos, a qualidade do código e sua documentação.
Opte por utilizar as seguintes linguagens de programação: Javascript, Python, C e C++.

Abaixo está um exemplo de entrada e saída para este desafio:
**Entrada:**

```json
[{"name":"Sapo", "priority": 7}, {"name":"Cachorro", "priority": 4}, {"name":"Coelho", "priority": 2}, {"name":"Vaca", "priority": 3},{"name":"Papagaio", "priority": 6},{"name":"Galinha", "priority": 5},{"name":"Gato", "priority": 1}]
```

**Saída:**

```json
[{"name":"Gato", "priority": 1}, {"name":"Coelho", "priority": 2}, {"name":"Vaca", "priority": 3}, {"name":"Cachorro", "priority": 4}, {"name":"Galinha", "priority": 5}, {"name":"Papagaio", "priority": 6}, {"name":"Sapo", "priority": 7}]
```