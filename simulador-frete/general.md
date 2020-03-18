# Dúvidas gerais

[filename](../_helpers/support-php.md ':include')

[filename](../_helpers/include-php.md ':include')

## Por que o simulador fica oculto para variações?

No WooCommerce cada variação pode ter peso, dimensões e valores diferentes. Dessa forma, se uma variação tiver 1kg e outra tiver 25kg, os custos de envio serão diferentes. Por isso o simulador de frete fica oculto até que uma variação seja selecionada.

Mas para produtos como camiseta o peso não muda, então os custos de envio também não. Nesse caso o simulador pode estar sempre visível.

!> Este comportamente pode ser alterado nas configurações do plugin.


## Ocultar o simulador em alguns produtos

Por padrão, o simulador será exibido em todos os produtos exceto se:

- Produto não precisa de entrega (digital, por exemplo)
- Produto está fora de estoque
- Produto é do tipo Grupo de Produtos ou Externo (link para outro site)

Então se você instalar plugins que adicionem métodos personalizados o plugin também funcionará. No entanto, alguns tipos de produto podem ter regras específicas ou funcionar com outros propósitos. Por isso você pode não precisar do simulador de frete neles.

Para incluir o tipo de produto customizado nas restrições basta usar o código abaixo:

```php
add_filter( 'wc_shipping_simulator_not_allowed_product_types', 'hide_wc_simulador_frete_types' );
function hide_wc_simulador_frete_types( $product_types ) {
  $product_types[] = 'simple';
  return $product_types;
}
```

No exemplo acima ocultamos o simulador para os produtos simples do WooCommerce. Basta mudar o nome `simple` pelo nome do seu tipo de produto personalizado.

## Alterar a mensagem para CEPs não cobertos

Quando algum CEP não está coberto nas configurações de área de entrega do seu site, a mensagem abaixo é exibida ao cliente:

![Tela de download](images/area-nao-coberta.jpg ':class=img50')

Para mudar isso, basta usar o código abaixo:

```php
add_filter( 'wc_simulador_frete_no_methods_available', 'wcsf_no_methods_message' );
function wcsf_no_methods_message( $message ) {
  return 'Seu CEP não está em nossa área de atendimento.';
}
```
