# Página de entrada do Grupo VIP (WhatsApp)

Página de um único arquivo (`index.html`), sem dependências, feita para celular.

## 1. Configurar
Abra o `index.html` e edite só o bloco `CONFIG` no topo:

- `grupos`: cole o(s) link(s) `https://chat.whatsapp.com/...`. Com mais de um, os visitantes são divididos entre eles, e cada pessoa sempre cai no mesmo grupo.
- `membros`: ex. `"+12 mil"`. Deixe `""` para não mostrar.
- `pixelMeta`: ID do Pixel do Facebook/Instagram Ads (opcional). Registra `PageView` e `Lead` no clique.
- `lojas`: lista de lojas exibidas.
- Prévia no WhatsApp: na linha `og:image` do `index.html`, troque `SEU-USUARIO` e `SEU-REPO` pelo seu endereço do GitHub Pages, para a imagem aparecer quando o link for compartilhado.

Dica: `seusite/?g=2` força o grupo 2 (bom para campanhas separadas).

## 2. Publicar no GitHub Pages
1. Em github.com → **New repository** → nome, ex.: `grupo-vip` → **Public** → Create.
2. **Add file → Upload files** → envie os 3 arquivos juntos: `index.html`, `mascote.webp` e `capa.jpg` → **Commit changes**.
3. **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `(root)` → **Save**.
4. Em 1–2 minutos o site fica em `https://SEU-USUARIO.github.io/grupo-vip/`.

### Domínio próprio (opcional)
Em **Settings → Pages → Custom domain**, coloque o domínio (ex.: `promo.seudominio.com.br`) e, no seu provedor de DNS, crie um registro **CNAME** apontando para `SEU-USUARIO.github.io`. Marque **Enforce HTTPS**.
