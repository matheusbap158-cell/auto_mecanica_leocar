# LeoCar Mecânica de Autos: landing page

Landing page em arquivo único (`index.html`). Oficina mecânica em Varginha/MG (Eldorado). Status: demo, não publicada.

## Como visualizar
Abra o `index.html` com duplo clique (caminhos relativos). O mapa da seção "Onde estamos" precisa de internet.

## Estrutura
- `index.html`: HTML + CSS + JS. Seções: hero com marcador de precisão (nota 5,0), faixa de números, a oficina, gráfico dos assuntos citados nas avaliações, avaliações, como funciona, sinais de alerta, montador de mensagem para o WhatsApp, onde estamos (com mapa), CTA final, rodapé e botão flutuante.
- `assets/favicon.svg`: ícone provisório (letra L).
- `Copy.txt`: texto da página (fonte da verdade).
- `design-system-leocar.html` (texto-fonte em `_fontes/`, oculta): design system.
- `Info maps.txt`: único material recebido (Google Maps).

## Pendências antes de publicar
- **WhatsApp:** o site usa o celular do Maps, (35) 98848-9917, sem confirmação de que é WhatsApp (`WA_NUMBER` no fim do `<script>`).
- **Logo e fotos da oficina:** não existem na pasta. O cabeçalho usa o nome escrito e há um bloco de foto tracejado.
- Instagram, lista de serviços, nome do responsável (as avaliações citam "Léo"), anos de oficina e horário completo (o Maps só mostra "Fecha 18:00").
- Autorização para citar as avaliações com nome abreviado.
- As cores (grafite e laranja) são proposta da agência, sem identidade da marca.
- O mapa é o embed do Google (não foi possível conferir a imagem no navegador de teste).
- Fontes carregadas do Google Fonts, como no design system. Ao publicar, incluir `og:image` com URL absoluta.
