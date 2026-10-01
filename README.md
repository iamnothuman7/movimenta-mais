# Movimenta Mais

Base de estudo derivada do [Astro Supabase Starter da Netlify](https://github.com/netlify-templates/astro-supabase-starter). O código atual demonstra a integração entre Astro, Supabase e Netlify; ainda não implementa um produto próprio completo chamado Movimenta Mais.

## Origem e tecnologias

A estrutura, exemplos e materiais do starter foram preservados. A autoria da base é de `netlify-templates`, conforme a [licença MIT](LICENSE). Este repositório não apresenta esse trabalho de terceiros como uma implementação original integral.

O projeto usa Astro, TypeScript, Tailwind CSS, o cliente JavaScript do Supabase e o adaptador Netlify. Consulte `package.json` e `package-lock.json` para as versões declaradas.

## Desenvolvimento local

Use uma versão de Node.js compatível com o Astro declarado no projeto.

```sh
git clone https://github.com/iamnothuman7/movimenta-mais.git
cd movimenta-mais
npm ci
npm run dev
```

A interface usa dados do Supabase. Para testar os fluxos completos, configure um projeto de desenvolvimento próprio, confira as migrações em `supabase/migrations/` e a carga de exemplo em `supabase/seed.csv`. Não aplique esses arquivos em um banco de produção.

Use `.env-example` como referência para `SUPABASE_DATABASE_URL` e `SUPABASE_ANON_KEY`. Guarde valores reais fora do Git; não substitua a chave anônima por uma chave administrativa no frontend. Consulte também [USAGE.md](USAGE.md) e os guias em `src/content/guides/`.

## Comandos

| Comando | Objetivo |
| --- | --- |
| `npm run dev` | Servidor de desenvolvimento Astro |
| `npm run build` | Verificação Astro e build |
| `npm run preview` | Pré-visualização local do build |

Recursos dependentes do ambiente Netlify podem exigir a configuração de desenvolvimento descrita nos guias do starter. Um build concluído não substitui testes de autorização, políticas do banco e integração. Não há suíte funcional dedicada no `package.json` atual.

## Evolução

Definir o domínio do produto, modelar suas entidades e criar testes são próximos passos de desenvolvimento, não funcionalidades já entregues. Alterações devem preservar a atribuição e a licença da base original.
