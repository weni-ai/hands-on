# Informações

- **Nome do Fluxo**: [Sienge] Consultar Saldo Devedor
- **Objetivo**: Esse fluxo tem como principal objetivo consultar o saldo devedor do cliente a partir do seu CPF

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro               | Descrição                                              |
|-------------------------|--------------------------------------------------------|
| cpf                     | CPF do cliente sem pontuação, por exemplo: 12365478912 |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado               | Descrição                   |
|-------------------------|-----------------------------|
| resposta                | Os dados completos do cliente, o formato dessa variável segue exatamente o mesmo retornado [pela API]. Acessível usando `@child.results.resposta.extra.[A PARTIR DAQUI É O RESULTADO DA API]` |

Documentação API Sienge
(https://api.sienge.com.br/docs/#/total-current-debit-balance-v1) 

GET /total-current-debit-balance/

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo: 

Exemplo de acesso: `@child.results.resposta.extra.results.0.totalCurrentDebitBalanceValue`

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>
