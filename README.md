# Ideias Cozy e Fofas

Webapp estatico para gerar ideias aleatorias de desenhos cozy e fofos sem repetir dentro da rodada atual.

## Publicar no Netlify

1. Envie esta pasta para um repositorio Git ou arraste a pasta no painel do Netlify.
2. Use estas configuracoes:
   - Build command: vazio
   - Publish directory: `.`
3. O arquivo `netlify.toml` ja define headers, cache e fallback para `index.html`.
4. O arquivo `.netlifyignore` impede que o PDF de referencia seja enviado no deploy.

## Dominio proprio

No painel do Netlify, abra `Site configuration > Domain management`, adicione seu dominio e siga os registros DNS indicados pelo Netlify. Depois que o DNS propagar, qualquer aparelho podera acessar o app pelo seu dominio.

## Editar prompts

As ideias ficam dentro do array `ideas` em `index.html`. Cada item usa:

- `title`
- `text`
- `palette`
- `challenge`
