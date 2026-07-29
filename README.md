# Foco no KM — Landing / Mídia Kit

Site estático de um arquivo só. Não precisa de build, npm nem framework.

## Arquivos
- `index.html` — a página inteira (CSS e fotos embutidos)
- `og-cover.jpg` — imagem que aparece no preview ao compartilhar o link
- `robots.txt`

## Antes de publicar
Abra `index.html` e troque **`foconokm.com.br`** pelo seu domínio real.
São 5 ocorrências, todas no topo do arquivo (bloco "EDITE AQUI").
No VS Code: Ctrl+H (Cmd+H no Mac), localizar `foconokm.com.br`, substituir por todos.

## Publicar no Cloudflare Pages (grátis)
1. `git init` / commit / push para um repositório no GitHub
2. Cloudflare > Workers & Pages > Create > Pages > Connect to Git
3. Framework preset: **None**. Build command: vazio. Output directory: `/`
4. Deploy
5. Custom domains > Set up a domain > digite seu domínio (o DNS já está na Cloudflare, ele configura sozinho)

## Testar local
No VS Code, extensão **Live Server** > botão "Go Live".
Ou: `python3 -m http.server 8000` e abrir http://localhost:8000
