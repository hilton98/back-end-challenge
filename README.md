# Instrução para uso:

Executar requisição com os valores de {amount} e {rate} separados por vírgula e não por pontos, exemplos:
* http://localhost:8000/exchange/10,1/BRL/USD/4,50
* http://localhost:8000/exchange/10,5/BRL/USD/4

# Back-end Challenge

Desafio para os futuros programadores back-end da Apiki.

## Introdução

Desenvolva uma **REST API** que faça conversão de moedas.

**Especifícações**:

* A URL da requisição deve seguir o seguinte formato:
   * http://localhost:8000/exchange/{amount}/{from}/{to}/{rate}
   * http://localhost:8000/exchange/10/BRL/USD/4.50
* A resposta deve seguir o seguinte formato:
   ```json
   {
     "valorConvertido": 45,
     "simboloMoeda": "$"
   }
   ```
* Conversões:
    * De Real para Dólar;
    * De Dólar para Real;
    * De Real para Euro;
    * De Euro para Real;
* Serão executados testes automatizados para validação dos requisitos:
   * Levantar servidor embutido do PHP: `php -S localhost:8000 index.php`;
   * Executando testes: `composer test`;
   * Executando lint: `composer lint`;

## Instruções

1. Efetue o fork deste repositório e crie um branch com o seu nome e sobrenome. (exemplo: fulano-dasilva)
2. Após finalizar o desafio, crie um Pull Request.
3. Aguarde algum contribuidor realizar o code review.
 
*Obs.: Não esqueça de executar o `composer test` e `composer lint` localmente.*

## Pré-requisitos

* PHP 7.4
* Orientado a objetos

## Dúvidas

Em caso de dúvidas, crie uma issue.
