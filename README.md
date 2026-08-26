# Cinco Salas

Escritório de produtos em planta baixa. Cinco SaaS, cada um numa sala com a
própria marca, mais **duas salas de reunião de uso comum**, ligadas por um
corredor e por um método.

No ar a partir da raiz — o site é estático, sem build.

## O desenho

**O corredor é acromático.** Toda a cor da página pertence a uma sala. O único
acento da casa é a luz que sai das janelas.

**As salas não seguem o tema do visitante.** Você entra na sala e a luz da sala é
a luz da sala: grafite e ciano, tinta e latão, papel e navy, quase-preto e rosé,
noite e laranja. Só o corredor troca de claro para escuro conforme o sistema.

**A área de cada sala de produto é proporcional a quanto de produto existe** lá
dentro — modelos, telas, testes, decisões registradas. As duas salas de reunião
ficam fora dessa conta: são de todos. A planta é desenho técnico de verdade:
parede cheia, giro de folha nas portas, mesa redonda com cadeiras nas salas de
reunião, hachura no corredor, cota, norte. As portas são escalonadas para
nenhuma alinhar com a da sala oposta.

**As salas de reunião não têm cor de dono.** A janela de cada uma é dividida nos
cinco tons, porque quem senta ali são os cinco.

## As salas

| # | Sala | Mercado | Estado |
|---|---|---|---|
| 01 | Carro do Freela | audiovisual · escala e contratação | protótipo, fora dos buscadores |
| 02 | Maestro | operação criativa · agência e cliente | em obra, 6 sprints concluídos |
| 03 | Disse Sim | cerimonial · três painéis | demonstração, dados fictícios |
| 04 | Pronta | maquiagem · o link na bio | protótipo, valores fictícios |
| 05 | MayHouse | contas da casa | no ar, 100% estático |

## As salas de reunião

| | Sala | Para que serve |
|---|---|---|
| A | **Marca** | A mesa onde as cinco identidades se sentam juntas: paletas, letra, piso de contraste, as palavras do produto. |
| B | **Máquina** | Infra, entrega e prova: onde cada um roda, como sobe, o que testa, o que instala no celular. |

O programa completo do escritório está em [`CLAUDE.md`](CLAUDE.md).

Os números e as regras de cada sala saíram da documentação de cada produto, e as
paletas saíram dos arquivos de token de cada um — não são aproximações.

## A tipografia

A casa fala em três vozes que não pertencem a nenhuma das salas: **Bricolage
Grotesque** nos rótulos de planta, **Newsreader** na prosa, **IBM Plex Mono** nas
cotas e nos fatos. Cada sala fala na letra da própria marca: Schibsted Grotesk,
Instrument Serif, Bodoni Moda, Baloo 2.

## Rodar

```bash
python3 -m http.server 4173
```

Não há dependências e não há build: `index.html` é o site inteiro, com os estilos
e o comportamento dentro. As fontes vêm do Google Fonts.

## Publicar

Importe o repositório na Vercel. Framework: *Other*. Build command e output
directory vazios — a raiz é o site.

## O pavimento em 3D

[`escritorio-3d.html`](escritorio-3d.html) — maquete navegável do pavimento
inteiro, 72 × 26 m, dezoito ambientes. Órbita com o mouse, e cada ambiente tem um
botão que leva a câmera para dentro dele.

Nenhuma sala tem parede: a zona é o **forro colorido suspenso** mais a **ilha de
carpete da mesma cor** no chão, exatamente embaixo. As cinco salas de produto
usam a cor da própria marca; a recepção, o convívio e as duas salas de reunião
recebem o forro em cinco faixas, porque são de todos.

**Toda mesa de reunião é retangular e longa, e nunca redonda** — as duas salas de
reunião são preparadas para podcast, com braços de microfone, feltro acústico e
tela. A cápsula *Máquina* é vidro curvo com cortina, solta no meio do pavimento.

Na ponta leste fica o **bloco de produção**: estúdio de foto e vídeo com fundo
infinito, camarim e cabine de edição. O estúdio abre direto no depósito de
equipamento, é o único ambiente sem forro — a laje aparente devolve 60 cm de
pé-direito para o grid de iluminação — e o bloco inteiro é sem cor, porque
parede colorida contamina o que se fotografa.

Three.js embutido no arquivo — sem CDN, sem build, abre offline.
