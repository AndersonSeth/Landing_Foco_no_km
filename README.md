# Foco no KM — Landing page / Mídia Kit

Site estático de arquivo único. Sem build, sem npm, sem framework.
Publicado via **GitHub Pages** em https://foconokm.com.br

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | A página inteira — CSS, fontes e fotos embutidos |
| `og-cover.jpg` | Imagem do preview ao compartilhar o link (WhatsApp, Instagram DM, LinkedIn) |
| `Midia-Kit-Foco-no-KM.pdf` | Versão em PDF, 7 páginas A4 |
| `robots.txt` | Libera indexação pelo Google |
| `CNAME` | Criado pelo GitHub — **não editar nem apagar** |

## Publicar uma alteração

```bash
git pull
git add .
git commit -m "descricao da alteracao"
git push
```

O GitHub Pages republica sozinho em 1–2 minutos.

## Testar antes de publicar
VS Code → extensão **Live Server** → botão "Go Live".
Ou: `python3 -m http.server 8000` e abrir http://localhost:8000

## DNS (já configurado, só para referência)
Registro.br → DNS → Editar Zona → Modo Avançado:

- 4 registros **A** na raiz: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- 1 registro **CNAME**: `www` → `andersonseth.github.io.`

GitHub: Settings → Pages → Custom domain `foconokm.com.br` + **Enforce HTTPS** ligado.

## Manutenção — o que atualizar a cada 3 meses
Os números do kit são de jul/2026. Quando exportar novos insights, os pontos a trocar em `index.html`:

- Bloco da capa: seguidores, views, contas alcançadas, múltiplo de alcance
- Página "Boletim": as 6 métricas e as leituras
- Página "Quem está do outro lado": gênero, faixa etária, cidades
- Página "Segunda tela": views, retenção, horas de exibição do YouTube
- Regerar o PDF: abrir o site no Chrome → Ctrl+P → Salvar como PDF → margens "Nenhuma" → marcar "Gráficos de segundo plano"
