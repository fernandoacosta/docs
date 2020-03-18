# Identificando problemas

Na esmagadora maioria dos casos o plugin funciona perfeitamente em qualquer loja, para qualquer tipo de produto. No entanto, falhas podem acontecer. Mas é possível corrigi-las.

Para isso, ative o log do plugin em WooCommerce -> Configurações -> Produtos -> Simulador de frete.

Acesse a página de um produto e faça uma simulação.

Pronto.

Agora um log com todas as informações será gerado em WooCommerce -> Status -> Logs -> `wc_simulador_frete`.

Copie todo o conteúdo do resultado, coloque no site Pastebin e me envie o link gerado. Com isso poderei auxiliar você na resolução desse problema.

## Alguns métodos não aparecem

Um problema comum é que alguns métodos não aparecem. No entanto, o problema quase nunca está no plugin.

Isso porque ele é feito para se integrar perfeitamente ao WooCommerce e todos os seus métodos.

Quando isso não acontece, faça o seguinte teste.

- Adicione ao carrinho o produto que está com problema
- Faça o teste diretamente na página do carrinho
- Certifique-se de que apenas um produto está no carrinho e está usando o mesmo CEP e quantidade (cenário idêntico entre página do produto e carrinho)

Com esse teste você consegue saber se o problema é no plugin ou no seu site. Se o método aparece no carrinho mas não no simulador, é algo no plugin e posso ajudar.

Caso não apareça nem no carrinho, é configuração do site e problema com tema/outros plugins e nesse caso não consigo ajudar como parte do suporte do plugin.

!> Um problema comum é PAC não aparecer quando o valor declarado está ativo e o preço do produto é menor que o mínimo exigido pelos Correios.
