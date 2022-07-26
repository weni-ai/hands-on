# Informações

- **Nome do Fluxo**: [Função] Atualizar KR na Qulture
- **Objetivo**: Atualizar uma métrica da Qulture com um novo valor

## Parâmetros

Parâmetros que são recebidos por esse fluxo para executar o seu objetivo. Os parâmetros desse fluxo são:

| Parâmetro                    | Descrição                                                                                                                 |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| data_kr                      | Data que a métrica vai ser atualizada, por exemplo: `@(now())` caso o valor não seja preenchido a data atual será passada |
| id_empresa                   | ID da Empresa na Qulture, normalmente pode ser capturado na URL ao abrir o sistema                                        |
| key_result_id                | ID da Métrica (Key Result) na Qulture que é capturado ao clicar nela e capturar na URL                                    |
| key_results_contribution_id  | ID da Contribuição da Métrica na Qulture que é capturado ao clicar nela e capturar na mesma URL da KR                     |
| token_qulture                | Token da Qulture que pode ser pego na configuração da sua organização dentro do sistema                                   |
| valor_kr                     | Número que vai ser passado para a métrica em formato decimal, por exemplo: 3.5                                            |

### Como configurar os parâmetros?

Quando escolher a ação "Entrar em outro fluxo" e você selecionar o fluxo que você quer executar, esses parâmetros podem ser preenchidos nessa aba:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/parametros.png?raw=true"/>

## Resultados

Resultados são respostas obtidas a partir da execução do fluxo. As respostas desse fluxo são:

| Resultado               | Descrição                   |
|-------------------------|-----------------------------|

### Como utilizar os resultados?

Para utilizar os seus resultados desse fluxo, você precisa utilizar a variável `@child.results.[NOME DO RESULTADO]`, substituindo `[NOME DO RESULTADO]` por um dos resultados acima e assim acessará o seu valor, como por exemplo:

<img src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true" data-canonical-src="https://github.com/weni-ai/hands-on/blob/main/assets/img/resultados.png?raw=true"/>
