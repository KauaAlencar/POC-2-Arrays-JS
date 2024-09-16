# **Manipulação de Arrays em JavaScript**

Este repositório contém uma demonstração de manipulação de arrays utilizando JavaScript. O projeto ilustra o uso de métodos como `sort()`, `map()`, `filter()` e `reduce()` para transformar e combinar arrays de forma eficiente.

### **Status do Projeto**

✅ **Projeto Concluído**

### **Pré-requisitos**

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com/), [Node.js](https://nodejs.org/en/).
Além disso, é bom ter um editor para trabalhar com o código, como [VSCode](https://code.visualstudio.com/).

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

O projeto é composto por uma única página HTML (`index.html`) que contém um exemplo prático de manipulação de arrays em JavaScript. Ele utiliza vários métodos do JavaScript para realizar operações em um array de números.

### **Conteúdo**

O código JavaScript utiliza os seguintes métodos para manipulação de arrays:

- **sort()**: Ordena os elementos de um array.
- **map()**: Cria um novo array com os resultados da aplicação de uma função em cada elemento.
- **filter()**: Cria um novo array com todos os elementos que passam em um teste.
- **reduce()**: Reduz o array a um único valor, acumulando os resultados.

### **Descrição das Operações**

1. **Ordenação e Transformação**

   O array inicial `numbers` é ordenado em ordem crescente. Em seguida, cada número é elevado ao quadrado e filtrado para manter apenas os valores maiores que 20.

   ```javascript
   const result = [...numbers]
       .sort((a, b) => a - b)
       .map(num => num * num)
       .filter(num => num > 20);
   ```

2. **Combinação de Arrays**

   O array original `numbers` é combinado com o resultado filtrado e transformado.

   ```javascript
   const combinedArrays = [...numbers, ...result];
   ```

### **Exemplo de Saída no Console**

- **Resultado Final**: Exibe o array transformado com valores filtrados maiores que 20.
- **Combined Arrays**: Exibe o array original combinado com os resultados.

### **Colaboradores**
   <table>
  <tr>
    <td align="center"><a href="https://github.com/usuario"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/xxxxxx?v=4" width="100px;" alt=""/><br /><sub><b>Seu Nome</b></sub></a><br /><a href="https://github.com/usuario" title="Github">🚀</a></td>
  </tr>
</table>

### **📝 Licença**

Este projeto está sob a licença MIT.
