8# Manipulação de Arrays em JavaScript

Este projeto ilustra o uso de métodos avançados para manipulação de arrays em JavaScript. Usando um exemplo prático, o código demonstra a aplicação dos métodos `sort`, `map`, `filter`, `reduce` e o operador spread para realizar operações comuns com arrays.

## Descrição

O código trabalha com um array de números e mostra como cada método pode ser utilizado:

- **`sort()`**: Ordena os elementos do array.
- **`map()`**: Cria um novo array aplicando uma função fornecida a cada elemento.
- **`filter()`**: Filtra os elementos do array com base em uma condição fornecida.
- **`reduce()`**: Reduz o array a um único valor com uma função acumuladora.
- **Operador spread**: Expande os elementos de um array em outro.

## Como Usar

1. Clone o repositório para sua máquina local:

    ```bash
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```

2. Acesse o diretório do projeto:

    ```bash
    cd nome-do-repositorio
    ```

3. Abra o arquivo `index.html` em um navegador de internet.

4. Abra o console do navegador (pressionando F12 ou clicando com o botão direito e selecionando "Inspecionar" -> "Console") para visualizar os resultados.

## Código HTML

O arquivo `index.html` contém o seguinte código:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manipulação de Arrays em JavaScript</title>
</head>
<body>
    <h1>Manipulação de Arrays em JavaScript</h1>
    <p>Abra o console do navegador para ver o resultado.</p>
    <script>
        const numbers = [10, 3, 7, 1, 9, 2, 8, 6, 4, 5];

        const result = [...numbers]
            .sort((a, b) => a - b)  
            .map(num => num * num) 
            .filter(num => num > 20) 
            .reduce((acc, num) => { 
                acc.push(num);
                return acc;
            }, []); 

        console.log('Resultado Final:', result);

        const combinedArrays = [...numbers, ...result];
        console.log('Combined Arrays:', combinedArrays); 
    </script>
</body>
</html>
```

## Conceitos Demonstrados

- **Ordenação de arrays** com `sort()`
- **Transformação de arrays** com `map()`
- **Filtragem de elementos** com `filter()`
- **Redução de arrays** a um único valor ou estrutura com `reduce()`
- **Combinação de arrays** usando o operador spread

## Tecnologias Utilizadas

- HTML
- JavaScript

## Licença

Este projeto está licenciado sob a [MIT License](https://opensource.org/licenses/MIT).

## Instruções Adicionais

- Substitua `https://github.com/seu-usuario/nome-do-repositorio.git` pelo URL do seu repositório no GitHub.
- Se necessário, adicione uma licença ao projeto e atualize o link da licença no README.
