# Conectar Elementor ao Mautic

## Rastrear e-mail em qualquer campo

Embora o plugin seja destinado a enviar formulários do Elementor pro Mautic, você pode querer iniciar o rastreio do usuário assim que ele preenche um e-mail, seja num campo de newsletter ou mesmo no checkout.

Para isso, basta adicionar o código abaixo ao seu site:

```javascript
<script>
  jQuery( document ).ready( function( $ ) {
    $( document.body ).on( 'change', 'input[type="email"]', function( event ) {
      mt( 'send', 'pageview', { 'email': $( this ).val(), 'dynamic_email': 1 } );
    });
  });
</script>
```

Este irá monitorar todos os campos de e-mail do site e atualizar no Mautic assim que ele for preenchido.

!> Por favor, note que isto é um recurso diretamente relacionado ao Mautic, não conectado ao plugin. Sendo assim, não está coberto por suporte/atualizações.

Não sabe como adicionar este código? O jeito mais fácil é instalar o plugin **Header and Footer Scripts**. Acesse o painel do seu site -> Plugins -> Adicionar novo e procure por ele. [Veja a página oficial para mais informações](https://br.wordpress.org/plugins/header-and-footer-scripts/).


----------

