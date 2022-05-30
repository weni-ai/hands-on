# Informações

**Nome do Fluxo**: [Função] Extrator de Informação.
**Objetivo**: Extrair informação de uma base de conhecimento do módulo de Inteligência Artificial da Plataforma Weni.

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro               | Descrição                                                                                                                                                                                                                   |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| access_token            | Token de acesso da Inteligência, copie e cole esse código: Abra o módulo Inteligência Artificial > Nova Inteligência de Conteúdo (ou uma já existente) > API > Access Token                                                 |
| confianca               | Percentual de confiança para aceitar uma resposta, coloque apenas um número, como por exemplo: 50                                                                                                                           |
| id_base_de_conhecimento | ID da Base de Conhecimento que você está extraindo informação, copie e cole esse código: Abra o módulo Inteligência Artificial > Nova Inteligência de Conteúdo (ou uma já existente) > API > POST Corpo > knowledge_base_id |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:
<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado               | Descrição                                                                                                                                                                                                                   |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| resposta                | Resposta extraída a partir da Base de Conhecimento que foi passada por parâmetro, caso não seja encontrada uma resposta ou ela não atenda o critério de confiança mínimo passado, a resposta será vazia                     |

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:
<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>