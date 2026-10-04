# Barbearia

Aplicativo de agenda em HTML, adaptado para celular e computador, com tema escuro.

## Publicar com GitHub Pages

1. Envie `index.html` para a raiz de um repositório GitHub.
2. Em **Settings → Pages**, selecione **Deploy from a branch**, a branch `main` e a pasta `/ (root)`.
3. Aguarde a publicação indicada pelo GitHub Pages.
4. O link de cliente usa o endereço publicado acrescido de `?acesso=cliente`.

O link de cliente abre a tela de boas-vindas e o formulário de reserva. O endereço pode incluir `&barbearia=Nome` para personalizar o título.

## Limite desta versão

GitHub Pages publica arquivos estáticos e não armazena dados compartilhados. Reservas ficam no armazenamento do navegador de quem as criou; assim, reservas feitas por clientes em outros dispositivos não aparecem automaticamente no Admin. Para sincronizar a agenda entre clientes e Admin, será necessário conectar um backend com banco de dados e autenticação.

O acesso Admin e os dados deste protótipo são locais e não devem ser tratados como segurança de produção.
