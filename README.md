# Brechó da Tati | Landing page catálogo

Site estático responsivo em HTML, CSS e JavaScript. Não precisa de Node, npm ou etapa de build para o GitHub Pages.

## Publicação no GitHub Pages

1. Crie um repositório no GitHub (por exemplo `brecho-da-tati`).
2. Envie os arquivos desta pasta para a raiz do repositório (`index.html`, `styles.css`, `script.js` e `assets/`).
3. Acesse **Settings > Pages > Build and deployment**.
4. Escolha **Deploy from a branch**, selecione `main` e `/ (root)`, depois salve.
5. Acesse `https://SEU-USUARIO.github.io/brecho-da-tati/` após a publicação.

## Personalização antes de publicar

### Contatos
No início de `script.js`, configure:

```js
const STORE = { whatsapp: '5511999999999', instagram: 'brechodatati' };
```

Substitua o número pelo WhatsApp real (DDI + DDD + número, sem espaços ou símbolos) e o Instagram pelo usuário real, sem `@` e sem espaços. Se esses campos ficarem vazios, o site exibirá uma mensagem informativa em vez de enviar o cliente para um contato inexistente.

### Produtos
No array `products` em `script.js`, substitua os **8 produtos demonstrativos**, preços, descrições e fotos por itens reais da loja. As fotos de exemplo são carregadas da internet (Unsplash). Para usar fotos próprias, salve em `assets/produtos/` e troque o campo `image` por `./assets/produtos/foto.jpg`.

### Banner e categorias
As imagens do banner e das categorias estão referenciadas no `index.html` e `styles.css`. Podem ser substituídas por fotos reais.

### Regras da loja
Informações incluídas: "Reutilizar é chique e sustentável", peças novas/seminovas, não realizamos trocas, pedidos via direct ou WhatsApp, novidades todo sábado.

## Funcionalidades
- Vitrine responsiva e filtros por categoria
- Ordenação por preço
- Favoritos salvos no navegador
- Modal de detalhes da peça
- Contato via WhatsApp com mensagem pré-preenchida
- Menu móvel e seções de banners, categorias, sobre e informações

**Importante:** este é um catálogo estático, não possui painel administrativo, banco de dados, checkout ou controle de estoque. Preços e produtos fornecidos são exemplos para demonstração.
