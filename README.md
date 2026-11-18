# Aula 5 - Atividades em C

Conjunto de atividades da aula 5, desenvolvidas em linguagem C. Os exercícios trabalham entrada e saída de dados, estruturas condicionais (`if`, `else if`, `else`) e `switch`.

## Atividades

| Arquivo | Tema | Recursos |
|---------|------|----------|
| `atividade1` | Raízes de equação do 2º grau | `float`, `math.h` (`sqrt`) |
| `atividade2` | Média de duas notas | `float`, `if` / `else` |
| `atividade3` | Aprovação por nota e frequência | `float`, `if` / `else if` / `else` |
| `aatividade5` | Valor total de hospedagem | `char`, `int`, `float`, `switch` |

### Atividade 1 - Equação do 2º grau

Lê os coeficientes `a`, `b` e `c` de uma equação do tipo `ax² + bx + c = 0`, calcula o discriminante (`delta = b² - 4ac`) e exibe as duas raízes com duas casas decimais.

### Atividade 2 - Média de duas notas

Lê duas notas, calcula a média aritmética e informa se o aluno foi aprovado (média maior ou igual a 6,0) ou reprovado.

### Atividade 3 - Aprovação por nota e frequência

Lê a média final e o percentual de frequência do aluno e informa a situação:

| Condição | Resultado |
|----------|-----------|
| Frequência menor que 75% | Reprovado por falta |
| Frequência de 75% ou mais e média menor que 6,0 | Reprovado por nota |
| Frequência de 75% ou mais e média de 6,0 ou mais | Aprovado |

A frequência é verificada primeiro, então a reprovação por falta vale mesmo com nota alta.

### Atividade 5 - Hospedagem

Lê o tipo de hospedagem e a quantidade de diárias, e calcula o valor total a pagar. Aceita letras maiúsculas e minúsculas. Se o tipo não for válido, exibe "Tipo invalido!!!" e encerra.

| Tipo | Valor da diária |
|------|-----------------|
| S | R$ 300,00 |
| D | R$ 450,00 |
| T | R$ 500,00 |

## Como compilar e executar

Os arquivos estão sem extensão. O mais simples é renomear para `.c`:

```bash
mv atividade1 atividade1.c
mv atividade2 atividade2.c
mv atividade3 atividade3.c
mv aatividade5 atividade5.c
```

Depois compile e execute (a atividade 1 precisa do `-lm`, por causa do `sqrt`):

```bash
gcc atividade1.c -o atividade1 -lm
gcc atividade2.c -o atividade2
gcc atividade3.c -o atividade3
gcc atividade5.c -o atividade5

./atividade1
```

## Exemplos de execução

**Atividade 2:**

```
Digite a primeira nota: 7
Digite a segunda nota: 8
Parabéns! Você foi aprovado com média 7.5
```

**Atividade 3:**

```
Qual a média final do aluno? 8
Qual o percentual de frequência? 70
O aluno foi reprovado por falta
```

**Atividade 5:**

```
Qual o tipo de hospedagem (S-D-T)? D
Qual a quantidade de diarias? 3
Valor total a pagar: R$ 1350.00
```
