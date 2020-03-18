# Personalizar plugin

O plugin possui um estilo básico com o objetivo de adaptar ao estilo padrão do seu site.

No final deste arquivo há uma customização padrão caso o seu tema não consiga apdatar a exibição.

!> O suporte não cobre personalizações e ajustes de CSS. Este documento serve apenas como referência.

## Mudar a cor do botão

```css
#wc-shipping-simulator .btn {
  background: #f00;
}
```

Basta trocar `#f00` pela cor que quiser.



## Estilo padrão.

Se precisar de um estilo profissional e não saiba como fazer, basta aplicar este CSS ao seu site:

```css
#wc-shipping-simulator {
  margin-bottom: 30px;
  margin-top: 30px;
}
#wc-shipping-simulator .cep-number {
  height: 40px;
  width: 45%;
  float: left;
}
#wc-shipping-simulator h3 {
  font-size: 16px !important;
  margin-bottom: 10px;
}
#wc-shipping-simulator .button {
  width: 50%;
  margin: 0 0 20px 15px;
  height: 40px;
  float: left;
  padding: 0;
  font-size: 16px;
  max-width: 120px;
}
#wc-shipping-simulator .button.loading {
  background-color: #000;
}
#wc-shipping-simulator .table-freight {
  width: 100%;
}
#wc-shipping-simulator .table-freight thead {
  background: rgba(233, 233, 233, 0.58);
}
#wc-shipping-simulator .table-freight th,
#wc-shipping-simulator .table-freight td {
  padding: 5px 10px;
}
#wc-shipping-simulator .table-freight tbody tr:nth-child(even) {
  background: rgba(233, 233, 233, 0.58);
}
#wc-shipping-simulator form {
  clear: both;
}
#wc-shipping-simulator form:before, #wc-shipping-simulator form:after {
  display: table;
  content: " ";
}
#wc-shipping-simulator form:after {
  clear: both;
}
```