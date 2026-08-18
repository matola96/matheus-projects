# Rumo ao Alvo 🎯🐢

Painel simples para vendedores acompanharem meta, super meta e vendas diárias.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público).
2. Faça upload do arquivo `index.html` deste zip para a raiz do repositório.
3. Vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/root` (ou `/(root)`).
5. Salve. Em alguns minutos o GitHub gera o link (algo como `https://seu-usuario.github.io/nome-do-repo/`).

## Sobre o armazenamento dos dados

Os dados (metas, vendas lançadas, diário) ficam salvos no **localStorage do navegador** — ou seja, gravados diretamente no navegador de quem está usando a página, não em um servidor.

Isso significa:

- Se o vendedor voltar outro dia **no mesmo navegador e no mesmo dispositivo**, a meta e o histórico continuam lá, exatamente como deixou.
- Cada vendedor cadastrado no seletor (+) tem seus próprios dados, isolados dos demais.
- Se o vendedor limpar os dados de navegação do navegador (cache/cookies/dados de sites), ou acessar de outro computador/celular, o histórico **não** aparece — porque ele nunca saiu daquele navegador.
- Não há sincronização entre dispositivos, porque este projeto é um arquivo único, sem banco de dados por trás.

Se no futuro for necessário que todos os vendedores vejam os dados de qualquer lugar (celular, outro computador, etc.), isso exige acrescentar um banco de dados/backend ao projeto.
