# Python Impressionador - Módulo 4

## Seus primeiros programas em Python

### Criando seu primeiro Programa

- [Cartilha - Primeiros Códigos em Python (Notebook)](./src/Cartilha%20-%20Primeiros%20Códigos%20em%20Python.ipynb)
- [Cartilha - Primeiros Códigos em Python (Código)](./src/cartilha_primeiros_códigos_em_python.py)
- [Meu Primeiro Programa - Olá Mundo!](./src/Primeiro_Programa.ipynb)

### Operações Básicas

No Notebook, para criar uma nova caixa de código, você pode utilizar o atalho "shift + Enter"

- [Operações Básicas](./src/Operacoes_Basicas.ipynb)

### Ordem das Operações no Python

Em Python, a ordem das operações matemáticas é tratada da mesma forma que aprendemos na matemática: seguindo a regra de precedência das operações. Em inglês, isso é frequentemente lembrado pela sigla PEMDAS:

- **P**arentheses (Parênteses)
- **E**xponents (Expoentes)
- **M**ultiplication and **D**ivision (Multiplicação e Divisão)
- **A**ddition and **S**ubtraction (Adição e Subtração)

Isso significa que operações dentro de parênteses são realizadas primeiro, seguidas pelos expoentes, depois a multiplicação e divisão (da esquerda para a direita), e finalmente a adição e subtração (da esquerda para a direita).

Aqui está um exemplo prático em Python:

```python
resultado = 2 + 3 * (2 ** 2) / 2 - 1
print(resultado)
```

No código acima, Python segue a ordem de operações da seguinte maneira:

1. Calcula o expoente: \(2 ** 2 = 4\)
2. Executa a multiplicação: \(3 * 4 = 12\)
3. Realiza a divisão: \(12 / 2 = 6\)
4. Adição e subtração: \(2 + 6 - 1 = 7\)

Portanto, o valor impresso seria 7.

### Operações com Texto (String)

- [Operações com Texto](./src/Operacoes_com_Texto.ipynb)

Em Python, operações com strings são extremamente poderosas e flexíveis. A seguir estão algumas das principais operações que podemos realizar com strings:

1. **Concatenar Strings**: Você pode combinar strings usando o operador `+`.
    ```python
    saudacao = "Olá, "
    nome = "Copilot"
    mensagem = saudacao + nome
    print(mensagem)  # Saída: Olá, Copilot
    ```

2. **Repetir Strings**: Use o operador `*` para repetir uma string várias vezes.
    ```python
    repeticao = "Oi! " * 3
    print(repeticao)  # Saída: Oi! Oi! Oi! 
    ```

3. **Acessar Caracteres e Slices**: Você pode acessar caracteres específicos ou fatias (slices) de uma string.
    ```python
    texto = "Python"
    primeiro_caractere = texto[0]
    slice_texto = texto[1:4]
    print(primeiro_caractere)  # Saída: P
    print(slice_texto)         # Saída: yth
    ```

4. **Funções de String**: Python possui diversas funções embutidas para manipulação de strings, como `lower()`, `upper()`, `strip()`, `split()`, `replace()`, entre outras.
    ```python
    texto = "   Aprendendo Python!  "
    texto_minusculo = texto.lower()
    texto_sem_espacos = texto.strip()
    lista_palavras = texto.split()
    nova_string = texto.replace("Python", "programação")

    print(texto_minusculo)  # saída: "   aprendendo python!  "
    print(texto_sem_espacos)  # saída: "Aprendendo Python!"
    print(lista_palavras)  # saída: ['Aprendendo', 'Python!']
    print(nova_string)  # saída: "   Aprendendo programação!  "
    ```

5. **Interpolação de Strings**: Em Python 3.6+, você pode usar `f-strings` para interpolar variáveis dentro de strings de forma mais limpa e legível.
    ```python
    nome = "Copilot"
    idade = 1
    mensagem = f"Meu nome é {nome} e eu tenho {idade} ano(s)."
    print(mensagem)  # Saída: Meu nome é Copilot e eu tenho 1 ano(s).
    ```

Operador `in` em Python é usado para verificar se uma substring está presente dentro de uma string, ou se um elemento está presente dentro de uma lista, tupla, ou outro tipo de coleção. Aqui estão alguns exemplos para ilustrar o uso do `in`:

### Verificar Substring em uma String
```python
frase = "O Python é incrível!"
if "Python" in frase:
    print("A palavra 'Python' está na frase.")  # Saída: A palavra 'Python' está na frase.
else:
    print("A palavra 'Python' não está na frase.")
```

### Verificar Elemento em uma Lista
```python
numeros = [1, 2, 3, 4, 5]
if 3 in numeros:
    print("O número 3 está na lista.")  # Saída: O número 3 está na lista.
else:
    print("O número 3 não está na lista.")
```

### Verificar Elemento em uma Tupla
```python
cores = ("vermelho", "verde", "azul")
if "azul" in cores:
    print("A cor azul está na tupla.")  # Saída: A cor azul está na tupla.
else:
    print("A cor azul não está na tupla.")
```

### Verificar Chave em um Dicionário
```python
aluno = {"nome": "Maria", "idade": 22, "curso": "Engenharia"}
if "idade" in aluno:
    print("A chave 'idade' está no dicionário.")  # Saída: A chave 'idade' está no dicionário.
else:
    print("A chave 'idade' não está no dicionário.")
```
