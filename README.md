# Central Psicopedagógica

Biblioteca digital (app web estático) da **Apostila Completa de Avaliação e
Intervenção Psicopedagógica 2026**. SPA mobile-first, dark premium, com dois
níveis de acesso (Apostila e Combo Profissional).

## Rodar localmente
Abra `index.html` no navegador (funciona offline, sem build).

## Publicar (GitHub + Vercel)
1. **Criar o repositório no GitHub** e subir este projeto (comandos abaixo).
2. **No Vercel** (vercel.com) → *Add New… → Project* → *Continue with GitHub* →
   *Import* o repositório `central-psicopedagogica`.
3. Framework Preset: **Other** · Build Command: *(vazio)* · Output Directory: *(vazio / raiz)*.
4. Clique **Deploy**. Em ~30s o site fica no ar com uma URL `*.vercel.app`.

> Site 100% estático: não precisa de build nem de `vercel.json`.
> Cada `git push` novo no GitHub re-publica automaticamente no Vercel.

### Subir para o GitHub por linha de comando
```bash
# 1) crie um repositório VAZIO no github.com (sem README)
# 2) rode, trocando SEU-USUARIO:
git remote add origin https://github.com/SEU-USUARIO/central-psicopedagogica.git
git push -u origin main
```

## O que ainda falta plugar
- **Links de download**: cada material está com `file: null`. Procure por
  `// COLAR LINK REAL AQUI` e por `data-arquivo` no `index.html`.
- **Controle de acesso**: o plano (Apostila x Combo) é escolhido em "Conta" e
  salvo no navegador (placeholder). Troque por login/verificação real de compra.
- **Itens NÃO IDENTIFICADOS**: os 20 jogos são placeholders; metadados do Kit
  Visual e separação das 1.500 atividades ficam marcados com `<!-- TROCAR -->`.

## Estrutura
```
index.html   app completo (HTML/CSS/JS em arquivo único)
img/         ilustrações 3D das seções
```
