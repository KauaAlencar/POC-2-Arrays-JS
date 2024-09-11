# Manipulação de Arrays em JavaScript

Este projeto demonstra o uso de métodos avançados de manipulação de arrays em JavaScript. O código integra os métodos `sort`, `map`, `reduce`, `filter` e o operador `spread` para realizar operações comuns com arrays.

## Descrição

O código manipula um array de números usando uma sequência de métodos JavaScript para demonstrar como cada um deles funciona:

1. **`sort()`**: Ordena os elementos do array em ordem crescente.
2. **`map()`**: Cria um novo array com os resultados da função fornecida aplicada a cada elemento do array original.
3. **`filter()`**: Cria um novo array com todos os elementos que passam em um teste fornecido.
4. **`reduce()`**: Reduz o array a um único valor ou estrutura usando uma função acumuladora.
5. **Operador `spread`**: Expande os elementos de um array para criar um novo array.

## Como Usar

1. Clone este repositório para a sua máquina local:

    ```bash
    git clone https://github.com/guilhermeshinohara/POC-2-Arrays-JS.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd POC-2-Arrays-JS
    ```

3. Abra o arquivo `index.html` em qualquer navegador de internet.

4. Abra o console do navegador (pressionando `F12` ou clicando com o botão direito e selecionando "Inspecionar" -> "Console") para visualizar os resultados.

## Código HTML

O arquivo `index.html` contém o seguinte código:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manipulação de Arrays em JavaScript</title>
</head>
<body>
    <h1>Manipulação de Arrays em JavaScript</h1>
    <p>Abra o console do navegador para ver o resultado.</p>

    <script>
        // Array inicial de números
        const numbers = [10, 3, 7, 1, 9, 2, 8, 6, 4, 5];

        // Usando todos os métodos em uma sequência
        const result = [...numbers]
            .sort((a, b) => a - b)  // 1. sort() - Ordenando os números em ordem crescente
            .map(num => num * num)  // 2. map() - Criando um novo array com cada número ao quadrado
            .filter(num => num > 20)  // 3. filter() - Filtrando os números que são maiores que 20
            .reduce((acc, num) => {  // 4. reduce() - Adicionando números ao acumulador
                acc.push(num);
                return acc;
            }, []); 

        console.log('Resultado Final:', result); // [25, 36, 49, 64, 81, 100]

        // 5. spread - Usando o operador spread para combinar o array original e o array resultante
        const combinedArrays = [...numbers, ...result];
        console.log('Combined Arrays:', combinedArrays); // [10, 3, 7, 1, 9, 2, 8, 6, 4, 5, 25, 36, 49, 64, 81, 100];
    </script>
</body>
</html>
**## Conceitos Demonstrados**

Ordenação de arrays com sort()
Transformação de arrays com map()
Filtragem de elementos com filter()
Redução de arrays a um único valor ou estrutura com reduce()
Combinação de arrays usando o operador spread

**## Tecnologias Utilizadas**
HTML
JavaScript

**##Contribuição**
Contribuições são bem-vindas! Para contribuir, siga estas diretrizes:

Adicione testes para novos recursos ou correções de bugs.
Garanta que o código esteja bem documentado.
Faça commits com mensagens claras e descritivas.
Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias ou correções.

**Licença**
Este projeto está licenciado sob a MIT License.
