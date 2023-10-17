- Quando programamos estamos lidando em geral com dois recursos do computador
    - Memória → Usada para armazenar dados
    - Processador (CPU) → Usado para realizar cálculos sobre os dados armazenados
- Por mais complexo que seja um código, um computador sempre vai realizar as seguintes operações:
    - Armazenar
    - Ler
    - Realizar operações com um ou dois elementos de cada vez

```python
a = 7
'''Computador pega o valor 7 e armazena enm algum lugar da sua memória, 
e esse local é identificado pela variável "a" '''
b = 5
'''Computador pega o valor 5 e armazena enm algum lugar da sua memória, 
e esse local é identificado pela variável "b" '''
a + b
''' o processador realiza uma operação de soma, buscando na memória os valores
identificados pelas variáveis a e b.
Nesse caso a soma é realizada,armazenada em algum lugal, mas como não estamos 
identificando esse local com uma variável não é armazenada a informação'''
c = a + b
''' Agora a operação é realizada, armazenada na memória e o local da memória que 
guarda o resultado dessa operação é identificado como sendo a variável "c"'''
```

- Ou seja, o recurso que gerenciamos enquanto programamos são: Memória e CPU do computador.
- Todo valor de um programa é atrelado em algum lugar da memória, mesmo temporareamente
- Uma váriável é uma forma de acesso ao local de memória que guarda um valor.
- Algumas instruções, mesmo que seja uma linha no código, pode ser desmembradas em várias tarefas de baixo nível para o computador.