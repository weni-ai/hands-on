# Informações

- **Nome do Fluxo**: [OpenAI] Text Completion.
- **Objetivo**: Integração com o Open AI - Text Completion.
- Pode ser usado para uma ampla variedade de tarefas. Ele fornece uma interface simples, mas poderosa para qualquer um dos modelos de texto do OpenAI. Você insere algum texto como um prompt e o modelo gerará uma conclusão de texto que tenta corresponder a qualquer contexto ou padrão que você forneceu. 

## Vídeo


## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro               | Descrição                                                                                                                                                                                                                   |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| promt            | Comando a ser enviado para a API do OpenAI                                                 |
| token            | Chave API do OpenAI - Você pode criar uma neste link https://beta.openai.com/account/api-keys                                                 |


### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado               | Descrição                                                                                                                                                                                                                   |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| data                | Resposta extraída a do retorno da API do OpenAI |

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>

### Como configurar o token

Para o fluxo funcionar é nescessario colocar o token do OpenAI na variável global `Openai Connect Api`.
