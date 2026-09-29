# Proposta Figital Celular

Apresentação animada, pensada para celular (mobile-first), que demonstra uma proposta de integração entre **Bling**, **Mercado Livre** e **Shopee** para a **Figital Celular**, com site e sistemas próprios.

O visual segue a identidade da marca: fundo preto, verde `#30d158`, detalhes dourados, fonte Inter, partículas flutuando e cards em estilo vidro.

> Os pedidos e valores exibidos no painel do celular são **simulados**, apenas para demonstrar como a solução funcionaria. Nenhuma API real é chamada.

---

## Ideia do projeto

Lojas que vendem em vários marketplaces costumam repetir trabalho: conferir pedidos em cada canal, atualizar estoque manualmente e correr o risco de vender um produto que já acabou.

A proposta mostra como uma integração própria resolve isso:

1. **Conectar:** Bling, Mercado Livre e Shopee ligados entre si.
2. **Sincronizar:** pedidos, estoque e preços atualizados em tempo real.
3. **Escalar:** novos canais e funções conforme a empresa cresce.

---

## Estrutura do projeto

```
figital-proposta/
├── index.html   # Apresentação completa (HTML + CSS + JavaScript)
└── README.md    # Documentação
```

Todo o projeto está em um único arquivo, sem subpastas e sem dependências externas de código.

| Arquivo | Função |
|---|---|
| `index.html` | Estrutura das telas (HTML), visual e animações (CSS) e efeitos interativos (JavaScript). |
| `README.md` | Explica como o projeto funciona. |

---

## Como o `index.html` funciona

### CSS
- **Variáveis de cor** no `:root` centralizam a identidade visual (verde, dourado, fundos e textos).
- **Cabeçalho fixo** com o logo da marca.
- **Cards em grade de 2 colunas**, usados nas integrações e nas entregas, com efeito de elevação ao passar o mouse.
- **Mockup de celular** com um painel de vendas ao vivo dentro dele.
- **Animações** com `@keyframes`: celular flutuando, indicador "ao vivo" piscando, entrada dos pedidos e botão pulsando.
- **Acessibilidade:** com `prefers-reduced-motion`, as animações são desligadas para quem prefere menos movimento.

### Telas (HTML)

| # | Seção | Conteúdo |
|---|---|---|
| 1 | **Capa** | Título, indicadores animados e o celular com o painel ao vivo. |
| 2 | **Integrações** | Bling, Mercado Livre, Shopee e outros canais. |
| 3 | **Como funciona** | Os três passos: Conectar, Sincronizar, Escalar. |
| 4 | **Entregas** | Integração própria, site sob medida, estoque unificado, painel de vendas e código pertencente à empresa. |
| 5 | **Bling** | Os planos do Bling e qual é o recomendado. |
| 6 | **Parceria** | Os dois formatos de trabalho propostos. |
| 7 | **Fechamento** | Convite para conversar. |

### JavaScript
- **Aparecer ao rolar:** um `IntersectionObserver` revela cada bloco quando ele entra na tela.
- **Barra de progresso** no topo, que acompanha a rolagem.
- **Contadores animados** nos indicadores da capa.
- **Feed de pedidos ao vivo:** a cada poucos segundos, um pedido de exemplo do Mercado Livre ou da Shopee aparece no celular, marcado como enviado ao Bling, e o total de vendas sobe.
- **Partículas de fundo** desenhadas em `<canvas>`, no mesmo estilo do site da marca.

---

## Tecnologias

- HTML5
- CSS3 (variáveis, grid, flexbox, animações, `backdrop-filter`)
- JavaScript puro (`IntersectionObserver`, `canvas`, `setInterval`)
- Fonte Inter (Google Fonts)

Nenhuma biblioteca ou framework é utilizado.

---

## Próximos passos possíveis

- Substituir os pedidos simulados por dados reais da API do Bling.
- Receber eventos do Mercado Livre e da Shopee por webhook.
- Adicionar os logos oficiais das marcas.
