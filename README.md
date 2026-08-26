# Cinco Salas

Escritório de produtos em planta baixa. Cinco SaaS, cada um numa sala com a
própria marca, ligados por um corredor e por um método.

No ar a partir da raiz — o site é estático, sem build.

## O desenho

**O corredor é acromático.** Toda a cor da página pertence a uma sala. O único
acento da casa é a luz que sai das janelas.

**As salas não seguem o tema do visitante.** Você entra na sala e a luz da sala é
a luz da sala: grafite e ciano, tinta e latão, papel e navy, quase-preto e rosé,
noite e laranja. Só o corredor troca de claro para escuro conforme o sistema.

**A área de cada sala é proporcional a quanto de produto existe** lá dentro —
modelos, telas, testes, decisões registradas. A planta é desenho técnico de
verdade: parede cheia, giro de folha nas portas, hachura no corredor, cota,
norte. As portas são escalonadas para nenhuma alinhar com a da sala oposta.

## As salas

| # | Sala | Mercado | Estado |
|---|---|---|---|
| 01 | Carro do Freela | audiovisual · escala e contratação | protótipo, fora dos buscadores |
| 02 | Maestro | operação criativa · agência e cliente | em obra, 6 sprints concluídos |
| 03 | Disse Sim | cerimonial · três painéis | demonstração, dados fictícios |
| 04 | Pronta | maquiagem · o link na bio | protótipo, valores fictícios |
| 05 | MayHouse | contas da casa | no ar, 100% estático |

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
