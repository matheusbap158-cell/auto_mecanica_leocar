# Design system: LeoCar Mecânica de Autos

Base: a pasta só tem o Info maps.txt (sem logo, fotos ou Instagram). A identidade abaixo é **proposta da agência**, comum em oficina, e deve ser ajustada quando o logo chegar.

## Tom visual em 3 linhas
1. Grafite profundo com laranja de sinalização: oficina, ferramenta, painel de carro.
2. Tipografia condensada em maiúsculas nos títulos, como plaqueta e painel; texto limpo no corpo.
3. O marcador de precisão (velocímetro) mostra a nota real 5,0; verde só nos botões de WhatsApp.

## 1. Cores
| Token | Hex | Uso |
|---|---|---|
| g-950 | #0B0E12 | Fundo principal, hero, rodapé |
| g-900 | #11151B | Seções escuras alternadas |
| g-800 | #181E26 | Cards e formulário sobre escuro |
| g-700 | #232B36 | Bordas e campos |
| or-500 | #FF6B1A | Destaque, faixa de números, botão laranja |
| or-400 | #FF8A47 | Hover |
| or-300 | #FFB07F | Texto de destaque sobre escuro |
| or-700 | #B54500 | Texto de destaque sobre fundo claro (contraste 4,9:1) |
| paper | #F1F3F6 | Seções claras |
| paper-200 | #DDE2E9 | Bordas claras |
| steel-600 | #4C5563 | Texto secundário sobre fundo claro |
| text | #F2F4F7 | Texto sobre escuro |
| muted | #A9B0BB | Texto secundário sobre escuro |
| wa-500 | #25D366 | Exclusivo dos botões de WhatsApp |
| wa-ink | #052E16 | Texto do botão de WhatsApp |

Regras: verde só no WhatsApp (na primeira dobra: botão do hero e botão flutuante; o do cabeçalho é laranja). Texto sobre laranja é sempre g-950.

## 2. Tipografia (Google Fonts)
- Títulos: **Barlow Condensed** (600, 700, 800), maiúsculas.
- Corpo: **Barlow** (400, 500, 600, 700).

| Nível | Desktop | Mobile | Peso | Entrelinha |
|---|---|---|---|---|
| H1 | 104 px | 50 px | 800 | 0,95 |
| H2 | 58 px | 36 px | 700 | 1,02 |
| H3 | 30 px | 30 px | 700 | 1,2 |
| Corpo | 18 px | 17 px | 400 | 1,65 |
| Etiqueta | 13 px | 13 px | 700 (espaçada, maiúsculas) | 1,2 |

## 3. Componentes
- **Botão WhatsApp:** fundo #25D366, texto e ícone #052E16, altura 56 px, cantos 10 px.
- **Botão laranja:** fundo #FF6B1A, texto #0B0E12 (cabeçalho e apoio).
- **Botão contorno:** borda branca 30%, hover laranja.
- **Campos:** fundo g-900, borda g-700, 52 px, foco/hover com borda laranja, erro com borda #FF6B4A e mensagem.
- **Cards:** fundo g-800, borda branca 12%, cantos 16 px.
- **Marcador de precisão:** arco laranja de 270 graus com agulha, que sobe até 5,0 ao carregar.
- **Gráfico de barras:** barras em degradê laranja, com o número real de avaliações.

## 4. Estética
- Cantos: 4 / 10 / 16 px.
- Brilho laranja suave em destaques; sem sombra preta pesada. Textura de listras diagonais discretas no hero.
- Espaçamento em escala de 8; seções com 96 px (desktop) e 60 px (mobile).
- Movimento sutil (agulha, barras, entrada ao rolar), tudo desligado com prefers-reduced-motion.

## 5. Conversão para o WhatsApp
- CTA no topo, hero, como funciona, sinais de alerta, atendimento e final, mais o botão flutuante.
- O montador de mensagem (modelo do carro + o que está acontecendo) entrega a conversa pronta.
- Prova social real: 5,0, 62 avaliações, assuntos mais citados e 3 avaliações literais.

## Tokens prontos (CSS)
```css
:root{
  --g-950:#0B0E12; --g-900:#11151B; --g-800:#181E26; --g-700:#232B36;
  --or-300:#FFB07F; --or-400:#FF8A47; --or-500:#FF6B1A; --or-600:#E05500; --or-700:#B54500;
  --paper:#F1F3F6; --paper-200:#DDE2E9; --steel-600:#4C5563;
  --text:#F2F4F7; --muted:#A9B0BB; --line:rgba(255,255,255,.12);
  --wa-500:#25D366; --wa-ink:#052E16; --alert:#FF6B4A;
  --font-display:'Barlow Condensed','Arial Narrow',sans-serif; --font-body:'Barlow',system-ui,sans-serif;
  --r-sm:4px; --r-md:10px; --r-lg:16px; --r-full:999px;
  --glow:0 0 44px rgba(255,107,26,.28);
}
```
