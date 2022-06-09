# Informações

- **Nome do Fluxo**: [Sienge] Adicionar telefone
- **Objetivo**: Esse fluxo tem como principal adicionar um novo telefone a um cadastro de um cliente, os telefones existentes permanecem e um novo é adicionado.

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro               | Descrição                                                                   |
|-------------------------|-----------------------------------------------------------------------------|
| cpf                     | CPF do cliente sem pontuação, por exemplo: 12365478912                      |
| telefone                | Telefone do cliente com DDI, DDD e sem pontuação, por exemplo: 558299999999 |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado               | Descrição                   |
|-------------------------|-----------------------------|
| status                  | Resultado da transação de adicionar telefone, Caso a adição do telefone seja bem sucedida, o status será `sucesso` e caso algum problema ocorra será `falha` |

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>
