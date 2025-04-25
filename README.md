# ML - Linguagem de Programação

## Descrição
`ML` é uma linguagem de programação simples com suporte a comandos básicos como `Print`, `Scan`, tipos de dados, operadores aritméticos e lógicos, controle de fluxo (como `if`, `while`, `for`), e organização de código com funções. A linguagem permite realizar operações simples, manipular variáveis e executar estruturas condicionais e de repetição.

## Funcionalidades

### Comandos

- **Print**: Exibe um texto na saída.
    ```plaintext
    Print: "Olá, Mundo!";
    ```

- **Scan**: Lê um valor de entrada e armazena na variável.
    ```plaintext
    Scan: "%int", x;
    ```

### Tipos de Dados

- **int**: Número inteiro (ex: `10`, `-3`).
- **double**: Número com casas decimais (ex: `3.14`).
- **String**: Texto (ex: `"olá mundo"`).
- **bool**: Valor lógico (ex: `true`, `false`).

### Operadores

- **Aritméticos**: `+`, `-`, `*`, `/`, `%`
- **Lógicos**: `&&`, `||`, `!`
- **Comparação**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Atribuição**: `=`, `+=`, `-=`, etc.

### Controle de Fluxo

- **If**: Condicional.
    ```plaintext
    If(condicao) { // código }
    ```

- **While**: Laço de repetição.
    ```plaintext
    While(condicao) { // código }
    ```

- **For**: Laço de repetição com inicialização, condição e iterador.
    ```plaintext
    for(inicializador, condicao, interator) { // código }
    ```

- **Break**: Sai de um loop.

### Declarações e Organização

- **function** / **def**: Define uma função.
    ```plaintext
    function minhaFuncao() { // código }
    ```

- **return**: Retorna um valor de uma função.
    ```plaintext
    return 10;
    ```

- **import** / **include**: Usa código de outro arquivo/módulo.
    ```plaintext
    import meuModulo;
    ```

### Extras Úteis

- **null**: Valor nulo (sem valor).
- **true / false**: Valores booleanos.
- **class / struct / object**: Definir tipos próprios (caso seja orientada a objetos).
- **main**: Ponto de entrada do programa, em linguagens como C/C++.

## Gramática

A gramática da linguagem `MinhaLing` foi definida usando ANTLR. Aqui estão os principais componentes da gramática:

- **Comandos**: A linguagem suporta comandos como `Print`, `Scan` e atribuições simples.
- **Estruturas de Controle**: Como `if`, `while`, `for`, e `break`.
- **Declarações**: Declaração de variáveis com tipos como `int`, `double`, `String` e `bool`.
- **Funções**: Declaração e definição de funções com `function` ou `def`.

## Exemplos

### Exemplo 1: Exibindo uma mensagem
```plaintext
Print: "Olá, Mundo!";
```

### Exemplo 2: Lendo uma variável e fazendo uma comparação
```plaintext
int x;
Scan: "%int", x;
If(x > 10) {
    Print: "Maior que 10!";
} else {
    Print: "Menor ou igual a 10!";
}
```

### Exemplo 3: Laços de repetição
```plaintext
int i = 0;
While(i < 5) {
    Print: i;
    i = i + 1;
}
```

### Exemplo 4: Função com retorno
```plaintext
function soma(int a, int b) {
    return a + b;
}

int resultado = soma(5, 10);
Print: "Resultado: ", resultado;
```

## Como Usar

1. **Compilação**: Compile o código fonte da linguagem com ANTLR e gere o parser para a linguagem `ML`.
2. **Execução**: Crie um interpretador ou máquina virtual que execute o código gerado pela gramática.

## Dependências

- ANTLR 4.x ou superior para gerar o parser e lexer.
- Linguagem de programação Java ou outra que suporte ANTLR para execução.

## Contribuição

Contribuições são bem-vindas! Para contribuir, basta fazer um fork do repositório, criar uma branch com suas mudanças e abrir um pull request.

---
