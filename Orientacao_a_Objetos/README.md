**Classes**: É uma estrututa para abstração de dados. Uma maneira de dizer a liguagem que você quer construir o seu próprio tipo. 

```python

class Passaro:
	pass
```

**Atributos**:  São “adjetivos”. Aquilo que é atribuido a algo, exemplo:  “ O passário preto” → Preto é um adjetivo referente a cor do passaro, nesse contexto “cor” é um atributo. Ou seja, atributos são variáveis internas de uma abstração de dados.

```python
class Passaro:
	assas = 2
	bico = 1
```

**Métodos:** São a abstração de processos de uma abstração de dados. “São funções internas da classe”

- Metodos podem manipular o estado dos atributos. No python isso acontece usando duas palavras específicas: **self** e **cls**

```python
class Passaro:
	estado = 'indefinido'

	def voar(self):
		self.estado = 'Voando'
		print(self.estado)
	
	def pousar(self):
		self.estado = 'Parado'
		print(self.estado)
```

**Instância**: Quer dizer um ”exemplo”, ou seja, a classe Passaros é uma abstração de pássaros reais, ela é genérica, já a instânica é **O** pássaro em questão. 

```python
p1 = Passaro()
p2 = Passaro()

p1.voar()
p1.estado() -> Voando

p2.estado() -> Indefinido
```

**self x cls:** Usamos self sempre que queremos falar com o exemplo ( instancia) e usamos cls quando queremos falar com a classe.

```python
class Fila:

	c_fila = []
	
	@classmethod
	def c_entrar(cls,obj):
		cls.c_fila.apped(obj)
		print(cls.c_fila)
	
	del __init__(self):
		self.s_fila = []
	
	def s_entrar(self,obj):
		self.s_fila.append(obj)
		print(self.s_fila)
```

### Tipos de Métodos:

- **Métodos de instância:**
    - Só funcionam com a classe instanciada
    - Manipulam atributos da instância
- **Métodos de classe:**
    - Funcionam a todo momento, até mesmo na instância
    - Manipulam atributos de classes
- **Métodos estáticos:**
    - Funcionam a todo momento
    - Não interagem com atributos
- **Métodos abstratos:**
    - Dizem a subclasse o que ela deve implementar

---

**Herança**: É uma concepção para resolver dois problemas:

- O reuso de tipos abstratos de dados
- Todos os tipos têm a mesma hierarquia e são independetes

Com isso, a herança permite que:

- Tipos de dados abstratos possam ser construidos para solucionar problemas
    - com isso atender novos requisitos
- Criar hierarquia de tipos
    - Tipos co-dependentes
- Reutilização de código

```python
class Pizza:
	pecacos = 8

@classmethod
def mudar_tamanho(cls, pedaços):
	cls.pedaços = pedaços

#Herança
class Mussarela(Pizza):
	... 
class Calabresa(Pizza):
	... 

# A classe abaixo recebe Pizza por associação 
class MeioAMeio(Mussarela,Calabresa)
```

**Polimorfismo**: Muda o comportamento de algo na classe que foi herdada. Ex: “sobrescrever” um método de uma classse é “Polimosrfismo”

```python
class Pizza:
	pedaços = 8

	@classmethod
	def mudar_tamanho(cls, pedaços)
		cls.pedaços = pedaços

	@staticmethod
	def ingredientes():
		return 'Ingredientes'

class Mussarela(Pizza):
	@staticmethod
	def ingredientes():
		return ['queijo','molho de tomate','oregano']
```

**Encapsulamento**: Atributo oculto do mundo,estado privado | Clientes da classe não podem modificar o Atributo | Por convensão devemos colocar ‘__atributo’