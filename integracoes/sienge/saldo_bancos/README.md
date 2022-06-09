# Informações

- **Nome do Fluxo**: [Sienge] Consulta Saldos dos Bancos
- **Objetivo**: Obter o saldo de uma conta corrente cadastrada no Sienge

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro        | Descrição                                                                                                                                                             |
|------------------|-----------------------------------------------------------|
| cod_empresa      | Código da empresa que possui conta corrente cadastrada    |
| data             | Data da movimentação bancára no formato YYYY-MM-DD        |
| numero_da_conta  | Número da conta corrente. Exemplo: 0000014123             |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado      | Descrição                                |
|----------------|------------------------------------------|
| saldo          | Saldo da conta corrente no dia informado |
| conta_corrente | Número da conta corrente consultada      |

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>
