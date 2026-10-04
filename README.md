# Barbearia

Aplicativo local de agenda e gestão para barbearia, em HTML responsivo e com tema escuro. A amostra também inclui cadastro empresarial, contabilidade simplificada e visão tributária demonstrativa.

## Contabilidade e tributação da amostra

- Cadastro da empresa: razão social, nome fantasia, CNPJ, situação, início, natureza jurídica, CNAEs, atividade, porte, município/UF, certificado A1 e saldos iniciais.
- Perfil inicial preenchido como barbearia MEI fictícia, com exemplos em todos os campos. O CNPJ é intencionalmente inválido para não representar uma empresa real.
- Receita de exemplo de aproximadamente R$ 5.500 mensais (cerca de R$ 66.000 em 12 meses), abaixo do teto MEI configurado de R$ 81.000; a folha considera apenas um empregado.
- Lançamentos de receitas, deduções, custos, pessoal, despesas, resultados financeiros, tributos, investimentos, financiamentos e aportes.
- Demonstrativos resumidos: DRE, DVA, fluxo de caixa operacional/de investimento/de financiamento, balanço patrimonial, indicadores e resumo mensal.
- Comparativo tributário ilustrativo, limites de faturamento configuráveis, calendário geral de obrigações, Livro Razão e histórico local.
- Doze meses de lançamentos demonstrativos são criados na primeira abertura. Atendimentos marcados como concluídos geram receita uma única vez.

Os dados empresariais e contábeis são exemplos editáveis; o DAS mensal é ilustrativo (referência de serviços em 2026), e os valores não constituem apuração ou orientação tributária. O limite MEI de R$ 81.000 é o parâmetro demonstrativo inicial e pode ser alterado na tela da empresa; a faixa de R$ 36.000 é somente meta mínima interna de faturamento, não um requisito legal do MEI. Não há banco de dados: agenda, perfil e lançamentos ficam em `localStorage` no navegador atual e podem ser incluídos no backup JSON.

## Publicar com GitHub Pages

1. Envie `index.html` para a raiz de um repositório GitHub.
2. Em **Settings → Pages**, selecione **Deploy from a branch**, a branch `main` e a pasta `/ (root)`.
3. Aguarde a publicação indicada pelo GitHub Pages.
4. O link de cliente usa o endereço publicado acrescido de `?acesso=cliente`.

O link de cliente abre a tela de boas-vindas e o formulário de reserva. O endereço pode incluir `&barbearia=Nome` para personalizar o título.

## Limite desta versão

GitHub Pages publica arquivos estáticos e não armazena dados compartilhados. Reservas ficam no armazenamento do navegador de quem as criou; assim, reservas feitas por clientes em outros dispositivos não aparecem automaticamente no Admin. O mesmo vale para dados empresariais e contábeis. Para sincronizar os dados, será necessário conectar um backend com banco de dados e autenticação.

O acesso Admin e os dados deste protótipo são locais e não devem ser tratados como segurança de produção.
