# Jogo de adivinhação

A proposta desse projeto é realizar um jogo de adivinhação simples utilizando python. O usuário deve digitar um número de 1 até 6, o computador irá aleatóriamente gerar um número e se o número digitador pelo usuário for o mesmo que o do computador, ele ganha, senão ele perde.
O jogo deve ser infinito, sendo apenas encerrado caso o usuário determinar.

# Proposta

Para fazer nosso jogo, vamos definir o que desejamos dele:

* Deve ser um jogo continuo. O jogo só será desativado caso o usuário especifique;
* O jogo deve ter tratamento de erros para caractéres inválidos;
* O usuário teve ter um sistema de pontos;
* Teve haver um sistema de vidas, onde o usuário perde uma vida para cada erro.
* O usuário poderá sair do jogo a qualquer momento que dele desejar.

## Identificação de usuário

### Escolha de nome de usuário

O jogo iá iniciar perguntando o nome do usuário:

![escolha_nome_1](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/escolha-nome-1.png)

### Tratamento de erro I: 

Caso o jogar digite um caracté que não seja alfabetico, será gerado um erro e entrará em um loop até que digite um nome válido.

![escolha_nome_2](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/escolha-nome-2.png)

### Formatação de nome:

Independente da forma que o usuário digite o nome dele, se houver apenas caractéres válidos, o código irá formatar o texto com a primeira letra maiúscula:

![escolha_nome_3](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/escolha-nome-3.png)
![escolha_nome_4](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/escolha-nome-4.png)
![escolha_nome_5](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/escolha-nome-5.png)

## Início do jogo

O jogo irá questionar ao usuário se ele deseja jogar:

![inicio_jogo_1](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/inicio_jogo_1.png)

### Tratamento de erro:

Caso o usuário entrar com uma opção diferente de "S" ou "N", o jogo entrará em um loop até que ele fornceça uma entrada válida:

![inicio_jogo_2](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/inicio_jogo_2.png)

Independente ser maiúsuclo ou minúsculo, o código irá aceitar a resposta, desde que seja ou 'S' ou 'N':

![inicio_jogo_3](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/inicio_jogo_3.png)

## Jogando...

O programa irá pedir para o usuário escolhe um número de 0 até 6:

![jogatina_1](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/jogatina_1.png)

### Tratamento de erros:

Se o usuário digitar um caractére que não seja um número, o jogo irá pedir para que seja digitado um número válido.
Se o usuário digitar um número menor que 0 ou maior que 6, o jogo irá pedir para que seja digitado um número válido.

![jogatina_2](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/jogatina_2.png)

A cada erro do usuário, ele perde uma vida. Quando as três acabam, o jogo pergunta se ele deseja jogar novamente. Caso ele digite que sim, o jogo irá dar 3 vidas para ele e será reiniciado, caso digite que não, o jogo se encerra.

![jogatina_3](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/jogatina_3.png)

Caso o usuário digite não:

![jogatina_4](https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/jogatina_4.png)

## Considerações finais

O jogo foi estruturado para que o usuário pudesse sair no momento em que quisesse. Independente do ponto em que está, se digitar "sair", o jogo irá ser encerrado.
Foi pensado também em métodos de tratamento de erros. Presumi que poderia ocasionalmente haver erros de digitação, por isso realizei diversos tratamentos de erros.

# Tecnologias utilizadas

* Jupyter Lab
* Python
* lib random 

# Autor

<a href="//https://www.linkedin.com/in/mikeias-o-5a4b2a184/"><img src="https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/linkedin.png" alt="linkedin" width="20"></a> <a href="mailto:mikeias.d.s.o@gmail.com"><img src="https://github.com/xpcosmos/simulador-de-dados/blob/main/assets/gmail.png" alt="gmail" width="20">

# Licença

MIT License

Copyright (c) 2021 xpcosmos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
