# Informações

- **Nome do Fluxo**: [Sienge][Principal] Retira segunda via do cliente.
- **Objetivo**: Obter o link do boleto de uma parcela consultando a API financeira do Sienge.

## Vídeo

<div align="left">
      <a href="https://www.youtube.com/watch?v=jYk0BWW5iUw">
         <img src="https://www.youtube.com/vi/jYk0BWW5iUw/0.jpg" style="width:30%;">
      </a>
</div>

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro               | Subfluxo                                            | Descrição                                                                                                                                                             |
|-------------------------|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| cpf                     | [Sienge] Valida CLiente                             | CPF do cliente que será consultado a segunda via do boleto                                                                                                            |
| customer_id             | [Sienge] Obtém a próxima parcela e gera segunda via | Código do cliente que será consultado a segunda via do boleto                                                                                                         |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Subfluxo                                            | Resultado  | Descrição                                                                                                                                                |
|-----------------------------------------------------|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Sienge] Valida CLiente                             | cliente    | Dados do cliente em formato json com os campos id, name e email. Caso o CPF não exista na base, a variável cliente será vazio.                           |
| [Sienge] Obtém a próxima parcela e gera segunda via | boleto     | Link do boleto em formato PDF. Caso o cliente não tenha parcelas ou boleto gerado, será alertado essa informação em mensagem de texto.                   |

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>
