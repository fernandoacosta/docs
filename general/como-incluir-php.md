# Como adicionar códigos ao meu site?

O jeito mais fácil: instale o plugin "Code Snippets" e seja feliz. Ele fará toda a gestão para você direto pelo painel.

!> Ao incluir códigos, certifique-se de que removeu o trecho `<?php` do início dele. Em 99% dos casos ele deve ser removido.

## Mais contextos.

Se você quer entender o conceito por trás, irei explicar a partir de agora.

A forma mais comum de se adicionar snippets personalizados ao seu site WordPress é editando o arquivo `functions.php` do seu tema. Isso pode ser bastante útil em alguns casos.

Se você quer, por exemplo, ocultar o menu do seu site, você pode adicionar um código personalizado no `functions.php` do tema sem grandes problemas.

No entanto, se você quer por exemplo oferecer frete grátis para compras acima de R$ 100,00 no WooCommerce você pode seguir um caminho um pouco diferente. Se você colar o código no mesmo `functions.php` do seu site funcionará perfeitamente.

Mas e se você decidir trocar de tema?

A remoção do menu que você fez será perdida. O que não é um problema, já que esta era uma personalização específica de layout, e provavelmente não serviria no novo tema. Mas e quanto ao frete grátis acima de R$ 100,00? Esta é uma função do site, não do tema em específico. Então deveria ser mantida mesmo após trocar o tema, certo? Já que a oferta continua. Mas ao trocar de tema ela também foi removida.

Por isso é importante separar o que deve ou não ir no `functions.php` do seu tema.

Uma alternativa é utilizar um plugin personalizado. Funciona basicamente como o `functions.php` do seu tema mas em um plugin. Você só precisa criar um arquivo com cabeçalho correto e fazer upload no seu servidor. Requer um conhecimento mínimo em programação.

Uma outra forma, esta sim muito simples e que não requer nenhum conhecimento técnico é adicionar um plugin que faça a gestão destes pequenos trechos de código. Onde você pode, dentre outras coisas, ativar ou desativar temporariamente, definir títulos e agrupar por categorias. Além de criar categorias para códigos que servem apenas em um tema específico ou são para todos o site como um todo. Ou ainda definir uma categoria "temporária" que deve ser ativada em determinados períodos do ano.

#### Configurar o Code Snippets

Se você não se sente confortável em mexer em arquivos do tema (e não recomendo), vá até o painel do seu site e instale o plugin **Code Snippets**.

Feito isso, será criado um item chamado “Snippets” no painel do seu WordPress. Os principais itens aí são “All Snippets”, onde você poderá ver todos os snippets já adicionados. Além da opção “Add New”, para adicionar novos códigos.

Há também a opção de importar snippets e configurar o plugin. Nas configurações há algumas coisas interessantes, mas não obrigatórias, que você pode ver depois.

Ao adicionar um novo snippet, terá que informar:

- Title: nome descritivo para informar o que este código faz – somente você verá isso
- Code: o código em si. Tome cuidado com isso, utilize apenas códigos de fontes confiáveis
- Description: detalhes do código, você pode salvar detalhes sobre de onde baixou, etc

Por fim, você pode simplesmente “Salvar alterações”, que vai deixar o snippet salvo mas inativo. Ou “Save Changes and Active”, que vai colocar o snippet pra rodar.

Abaixo disso você também definir se o código deve ser sempre carregado ou selecionar se deve ser carregado no admin ou front end. Na dúvida, deixe marcado para carregar em todos os locais.

Pronto! Você já tem seus snippets funcionando e organizados. Sem risco de perdê-los ao atualizar o tema.

!>Os snippets adicionados pelo plugin são salvos no banco de dados, então é recomendável que você faça backups frequentes. Se você ainda não faz backups frequentes, recomendo começar imediatamente.
