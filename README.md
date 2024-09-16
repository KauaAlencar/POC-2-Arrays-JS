# **Manipulação de Arrays em JavaScript**

Este repositório contém uma demonstração prática de manipulação de arrays em JavaScript. O projeto exemplifica como usar métodos como `sort()`, `map()`, `filter()` e `reduce()` para realizar transformações e combinações eficientes de arrays.

### **Status do Projeto**

✅ **Projeto Concluído**

### **Pré-requisitos**

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com/), [Node.js](https://nodejs.org/en/).
Além disso, é recomendável ter um editor de texto para trabalhar com o código, como o [VSCode](https://code.visualstudio.com/).

### **🎲 Rodando o Projeto**

```bash
# Clone este repositório
$ git clone <https://github.com/KauaAlencar/POC-2-Arrays-JS>

# Acesse a pasta do projeto no terminal/cmd
$ cd POC-2-Arrays-JS

# Abra o arquivo index.html no seu navegador
# ou utilize uma extensão como Live Server no VSCode para rodar a aplicação.

```

### **Estrutura do Projeto**

O projeto é composto por uma única página HTML (`index.html`) que contém um exemplo prático de manipulação de arrays usando JavaScript. Ele demonstra a aplicação de diferentes métodos do JavaScript para manipular um array de números.

### **Conteúdo**

O código JavaScript utiliza os seguintes métodos para manipulação de arrays:

- **sort()**: Ordena os elementos do array de acordo com a função de comparação fornecida.
- **map()**: Aplica uma função a cada elemento do array, criando um novo array com os resultados.
- **filter()**: Filtra os elementos do array com base em uma condição, retornando um novo array contendo apenas os elementos que passaram no teste.
- **reduce()**: Acumula os valores do array em um único resultado, conforme uma função de acumulação especificada.

### **Descrição das Operações**

1. **Ordenação e Transformação dos Números**
    
    Primeiro, o array `numbers` é ordenado em ordem crescente utilizando o método `sort()`. Cada número é, então, elevado ao quadrado através do método `map()`. Por fim, apenas os números maiores que 20 são mantidos no array resultante, utilizando o método `filter()`.
    
    ```jsx
    const result = [...numbers]
        .sort((a, b) => a - b)  // Ordena os números em ordem crescente
        .map(num => num * num)  // Eleva cada número ao quadrado
        .filter(num => num > 20);  // Mantém apenas números maiores que 20
    
    ```
    
2. **Redução do Array com `reduce()`**
    
    O método `reduce()` é usado para acumular os resultados dentro de um novo array. Aqui, ele adiciona cada número que passou pela filtragem ao array final `result`.
    
    ```jsx
    .reduce((acc, num) => {
        acc.push(num);  // Acumula os números filtrados em um novo array
        return acc;
    }, []);
    
    ```
    
3. **Combinação de Arrays**
    
    O array original `numbers` é combinado com o array resultante (`result`), criando um novo array que contém tanto os números originais quanto os números filtrados e transformados.
    
    ```jsx
    const combinedArrays = [...numbers, ...result];  // Combina os dois arrays
    
    ```
    

### **Exemplo de Saída no Console**

- **Resultado Final**: Um array contendo os números do array original que, após serem elevados ao quadrado, são maiores que 20.
- **Combined Arrays**: Um novo array que combina os valores do array original com os números que foram transformados.

**Colaboradores**
     <table>
  <tr>
    <td align="center"><a href="https://github.com/KauaAlencar"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/172075258?v=4" width="100px;" alt=""/><br /><sub><b>Kauã Alencar</b></sub></a><br /><a href="(https://www.linkedin.com/in/kau%C3%A3-alencar-b15119215/)" title="Linkedin">🚀</a></td>
   <td align="center"><a href="https://github.com/GuilhermeShinohara"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/180458966?v=4" width="100px;" alt=""/><br /><sub><b>Guilherme Shinohara</b></sub></a><br /><a href="https://github.com/GuilhermeShinohara" title="Linkedin">🚀</a></td>
   <td align="center"><a href="https://github.com/LeoFavaron"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/179886009?v=4" width="100px;" alt=""/><br /><sub><b>Leonardo Favaron</b></sub></a><br /><a href="https://github.com/LeoFavaron" title="Linkedin">🚀</a></td>
   <td align="center"><a href="https://github.com/lucas-ricci-pathbit"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/174811028?v=4" width="100px;" alt=""/><br /><sub><b>Lucas Ricci</b></sub></a><br /><a href="https://github.com/lucas-ricci-pathbit" title="Linkedin">🚀</a></td>
    
  </tr>
</table>

### **📝 Licença**

Este projeto está sob a licença MIT. 
| Método | Descrição |
| --- | --- |
| **sort()** | Ordena os elementos do array de acordo com a função de comparação fornecida. |
| **map()** | Aplica uma função a cada elemento do array, criando um novo array com os resultados. |
| **filter()** | Filtra os elementos do array com base em uma condição, retornando um novo array contendo apenas os elementos que passaram no teste. |
| **reduce()** | Acumula os valores do array em um único resultado, conforme uma função de acumulação especificada.
 |
| **order** | Controla a ordem dos itens no container, permitindo reordenar os itens visualmente. |
| **flex-wrap** | Decide se os itens devem quebrar para a próxima linha quando não há espaço suficiente, ou se devem permanecer em uma única linha. |
