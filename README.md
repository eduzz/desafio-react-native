# Desafio React Native | Banco Virtual

Martha gostaria de ter um aplicativo que a permita inserir um valor (em reais) para saque e ela deseja que essa aplicação mostre o mínimo de cédulas disponíveis para o valor informado.

Esse aplicativo deve possuir duas telas: __caixa eletrônico__ e __extrato de movimentações financeiras__.

<p>&nbsp;</p>

## Tela de Caixa Eletrônico

A tela de caixa eletrônico é responsável por receber o valor que Martha gostaria de sacar e exibir para ela o mínimo de cédulas para saque. Para isso, o aplicativo deve seguir as seguintes regras de negócio:

1. Existem apenas as seguintes notas para saque: R$ 20, R$ 50 e R$ 100;
2. O usuário só poderá sacar a quantia de R$ 10.000 entre 08h00 até 17h00 e, após esse horário, o valor é limitado para R$ 3.000 por questões de segurança;
3. O aplicativo deve retornar sempre o menor número de cédulas possíveis;
4. Ao fazer um saque, adicionar ao extrato de movimentações financeiras o valor, data e hora da transação.

### Exemplos:
- Martha deseja sacar o valor de R$ 120,00. O aplicativo deve retornar que ela receberá 1 nota de R$ 100,00 e outra de R$ 20,00;
- Martha deseja sacar o valor de R$ 130,00. O aplicativo deve retornar um erro;
- Martha deseja sacar o valor de R$ 150,00. O aplicativo deve retornar que ela receberá 1 nota de R$ 100,00 e outra de R$ 50,00.

<p>&nbsp;</p>

## Tela de Extrato de Movimentações Financeiras

A tela de extrato de movimentações financeiras deve listar para Martha todos os saques realizados por ela. Esta tela deve conter obrigatoriamente:

- Uma listagem de todos os saques de Martha, por ordem decrescente de data;
- Cada transação deve ter o valor de saque realizado, juntamente com a data e hora;
- Um filtro por período de data dos saques.

<p>&nbsp;</p>

## Requisitos técnicos

O aplicativo deve, __obrigatoriamente__:
- Ser feito utilizando React Native;
- Utilizar TypeScript.

Você é livre para criar a interface do aplicativo da forma que desejar e utilizar as bibliotecas e frameworks adicionais de sua preferência, desde que siga os requisitos obrigatórios acima.

Você deve consumir a API que está [na pasta api](https://github.com/eduzz/desafio-react-native/tree/master/api) deste repositório, para buscar e inserir os dados das transações financeiras. Para mais informações sobre a API, leia o README.md da pasta api.

<p>&nbsp;</p>

## Entrega do desafio

Para realizar a entrega do desafio, você deve publicar seu código em um repositório do GitHub. Este repositório deve estar __público__ e deve conter as instruções mínimas para rodar o projeto.
