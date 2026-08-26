# Cinco Salas — o programa do escritório

Contexto permanente deste repositório. Quem mexer na planta ou nas seções lê
isto antes.

## O que o escritório é

Um hub de produtos: cinco SaaS independentes, cada um com marca própria, num
único pavimento. O site é a planta baixa desse pavimento, navegável.

## O programa

**Sete salas ao todo: cinco de produto e duas de reunião.**

### Salas de produto — uma por empresa, cada uma com a própria marca

| # | Sala | Mercado | Endereço | Estado |
|---|---|---|---|---|
| 01 | Carro do Freela | audiovisual · escala e contratação | carrodofreela.com.br | protótipo, `noindex` |
| 02 | Maestro | operação criativa · agência e cliente | maestroapptest.vercel.app | em obra, 6 sprints |
| 03 | Disse Sim | cerimonial · três painéis | dissesimapp.vercel.app | demonstração |
| 04 | Pronta | maquiagem · o link na bio | prontaapp.vercel.app | protótipo |
| 05 | MayHouse | contas da casa | mayhouse-vert.vercel.app | no ar |

### Salas de reunião — de uso comum dos cinco

**Não pertencem a nenhum produto e não têm marca própria.** São neutras de
propósito: a cor delas é a luz da casa (`--luz`), e a janela de cada uma é
dividida nos cinco tons, porque quem as usa são os cinco.

| | Sala | Para que serve |
|---|---|---|
| A | **Marca** | A mesa onde as cinco identidades se sentam juntas. Paletas, letra, piso de contraste, as palavras do produto. O que se decide aqui é o método, nunca o gosto de um produto sobre o outro. |
| B | **Máquina** | Infra, entrega e prova. Onde roda, como vai ao ar, o que os cinco testam, o que instala no celular. |

As duas regras da casa que sobram — a tese *decisão no lugar de conversa* — não
moram em sala nenhuma: fecham a página, porque valem para o pavimento inteiro.

## As regras do desenho

- **O corredor é neutro.** A cor da casa é a soma da cor das cinco salas de
  produto; a casa não tem acento próprio além da luz de janela.
- **As salas de produto não seguem o tema do visitante.** Cada uma renderiza no
  próprio mundo de marca. Só o corredor, o hall e as salas de reunião trocam de
  claro para escuro.
- **A área de cada sala de produto é proporcional a quanto de produto existe**
  lá dentro. As salas de reunião ficam fora dessa conta — são de todos.
- **O trilho da barra fixa repete essa proporção.** É a planta achatada em
  navegação.
- As portas são escalonadas: nenhuma alinha com a da sala oposta.
- Paletas e números vêm dos arquivos de token e da documentação de cada
  produto — nunca de estimativa.

## A tipografia

A casa fala em três vozes que não pertencem a nenhuma sala: **Bricolage
Grotesque** nos rótulos de planta, **Newsreader** na prosa, **IBM Plex Mono** nas
cotas. Cada sala de produto fala na letra da própria marca: Schibsted Grotesk,
Instrument Serif, Bodoni Moda, Baloo 2.

## Técnico

`index.html` é o site inteiro — estilos e comportamento dentro, sem build e sem
dependências. Fontes pelo Google Fonts. Publica na Vercel a partir da raiz.

---

# O programa expandido — LIBERADO EM 26/08/2026

> Registrado como briefing e liberado pelo Victor na mesma data. É este o
> programa que a vista 3D materializa.

## O norte

> "Estou materializando o meu sonho ideal."

Não é um site institucional: é o escritório que ele quer ter. As decisões devem
servir a isso — o desejo vem antes do argumento de produto.

## O que ele pediu

**1 · Demonstração em imagem das salas, em ponto de vista de quem está dentro.**
Não é mais planta baixa vista de cima: é a sala como ele a veria se estivesse ali
— "como se eu tivesse vendo elas".

**2 · Tipologia de planta aberta.** Salas mais abertas, no lugar de caixas
fechadas por parede cheia. Isso muda a planta atual: as sete salas foram
desenhadas como salas fechadas com porta e giro de folha.

**3 · Programa novo, a acrescentar ao existente:**

| Ambiente | Observação do pedido |
|---|---|
| Recepção | pedida na segunda rodada |
| Espaço de convívio | de uso mútuo do HUB, comum aos cinco produtos |
| Local de despressurização | descompressão, descanso |
| Copa | para café |
| Local para almoço | refeição |

Somados às sete salas já desenhadas (cinco de produto + duas de reunião,
*Marca* e *Máquina*), o pavimento tem **doze ambientes** e passa a ter área
social além da área de trabalho.

**4 · A mesa de reunião — regra dura.**

> "Não gosto das mesas redondas pra reunião, elas precisam ser horizontais mesmo,
> com possibilidade de virar podcast também."

**Nenhuma mesa de reunião é redonda.** Todas são retangulares e longas, no eixo
horizontal da sala. As duas salas de reunião são **preparadas para podcast**:
braços de microfone articulados, microfones, painéis de feltro acústico e tela.
A cápsula *Máquina* é o estúdio completo; *Marca* tem a mesma mesa e os mesmos
braços, sem o tratamento acústico pesado.

Isso derruba a mesa redonda que estava desenhada na planta 2D — lá ela era o
símbolo arquitetônico convencional de sala de reunião. **A planta 2D precisa ser
corrigida junto**, senão contradiz o 3D.

**5 · Liberdade criativa autorizada.** "Enfim, seja criativo."

## Referências

**Recebidas em 26/08/2026 — cinco imagens**, guardadas em
[`referencias/`](referencias/LEIA.md) com a leitura de cada uma.

O que elas resolvem, em uma linha: **a zona é definida por forro colorido
suspenso mais ilha de carpete da mesma cor no chão, nunca por parede.** É a
resposta à planta aberta, e encaixa no desenho atual porque cada sala do HUB já
tem uma cor — a planta perde as paredes sem perder as salas.

Duas coisas a não confundir:

- **A paleta das referências (azul, laranja, amarelo) é método, não cor.** A cor
  do HUB vem dos cinco produtos e não se troca; o corredor é neutro justamente
  para caber as cinco.
- **O recorte das referências é orgânico**, e a planta atual é desenho técnico
  reto. As duas linguagens não convivem bem na mesma página — é decisão a tomar,
  não detalhe.

## Como foi resolvido

- **A vista 3D convive com a planta**, em página própria (`escritorio-3d.html`),
  linkada do índice. A planta 2D continua carregando a regra "área = quanto de
  produto existe"; o 3D carrega o espaço.
- **Percurso, não vitrine.** Uma única maquete navegável do pavimento inteiro,
  com câmera que voa para dentro de cada ambiente. Nada de doze imagens soltas.
- **Os ambientes de uso comum não têm cor de dono.** Recepção, convívio e as duas
  salas de reunião recebem o forro em cinco faixas — as cinco marcas juntas.
  Copa e refeitório ficam em terracota, e a despressurização em grafite: são os
  únicos dois tons da casa que não pertencem a produto nenhum.
- **A planta é reta; o mobiliário e os forros são arredondados.** O desenho
  técnico continua ortogonal, e a curva entra no objeto — forro de canto redondo,
  cápsula de vidro curvo, ilha de carpete de canto suave.

## O pavimento — 15 ambientes

Placa de **64 × 26 m**, pé-direito 3,60 m, forros suspensos a 2,90 m. Uma espinha
de circulação leste-oeste no meio (z 11,5–14,5), sem forro, cortando o pavimento
inteiro, **com porta de vidro nas duas pontas** — ela terminava em parede cega.
Perímetro todo em vidro nas duas faces longas.

**Nenhuma sala de trabalho tem parede.** O único bloco de parede cheia é o
serviço: banheiro é a única coisa que a planta aberta não resolve. A planta 2D
foi redesenhada para parar de desenhar parede onde não há.

| Faixa | Ambiente | x | Cor |
|---|---|---|---|
| norte | Recepção | 1–10 | cinco faixas |
| norte | 01 Carro do Freela | 10,5–21 | ciano `#17D1E8` |
| norte | 02 Maestro | 21,5–33,5 | latão `#C8963A` |
| norte | 03 Disse Sim | 34–43,5 | navy `#064675` |
| norte | A · Marca (reunião) | 44–55 | cinco faixas |
| sul | Despressurização | 1–9,5 | grafite |
| sul | Convívio · a praça | 10–21,5 | carvalho + cinco faixas |
| sul | 04 Pronta | 22–30 | rosé `#EDB3BC` |
| sul | 05 MayHouse | 30,5–38,5 | laranja `#E08700` |
| sul | B · Máquina (cápsula podcast) | 39–46,5 | cinco faixas |
| sul | Copa | 47–55, z 14,5–19 | terracota |
| sul | Refeitório | 47–55, z 19–25 | terracota |
| norte | **Serviço** · feminino, masculino, acessível | 44–54 | bloco fechado |
| sul | **Despensa** · alimentos e limpeza | 55,5–63, z 14,5–19 | bloco fechado |
| sul | **Depósito** · equipamento audiovisual e técnico | 55,5–63, z 19–25 | bloco fechado |

Marca passou para 54,5–63. Serviço abre numa antecâmara, e a antecâmara abre no
corredor: ninguém entra em sanitário direto do aberto. Despensa encosta na copa
parede a parede — quem repõe o café não atravessa o escritório com a caixa.
Depósito é separado da despensa de propósito: câmera não se guarda ao lado de
material de limpeza.

## Os manuais de identidade — a fonte das cinco marcas

Lidos em 26/08/2026, direto do repositório de cada produto. **São eles que mandam,
não a estimativa.**

| Marca | Manual | O que ele corrigiu aqui |
|---|---|---|
| Carro do Freela | `app/public/identidade.html` (direção B, v1) | grafite é `#0E1216` (frio, de monitor calibrado) e cal é `#E9EEF0`. Símbolo: três lâminas, grid 100×100, alturas 52, larguras 7/13/26, opacidades 34/64/100%, skew −12°. Logotipo Schibsted Grotesk Black, **caixa alta e baixa**, tracking −0,045em. |
| Maestro | `docs/BRAND/VISUAL_IDENTITY.md` | Símbolo "M Batuta", path canônico `M11 35.5V12.5Q24 48.5 37 12.5V35.5`, traço 6, grid 48. Wordmark Instrument Serif Regular, tracking positivo. **Nunca "MAESTRO", nunca "maestro".** Canvas é `#08090B`. |
| Disse Sim | `src/marca/caminhos.ts` + `Logo.tsx` | Vetor oficial, medido contra o original. O "s" espelhado em "disse" é de propósito: com o "s" normal ao lado, os dois fazem um coração. Navy `#064675`, azul `#005C95`, reverso `#7FB6DC`. |
| Pronta | `marca/manual.html` (v2) | Um átomo só: o ponto de champanhe. Halo de 1,5× o raio, nunca mais. Logotipo Bodoni Moda 500, −0,026em, ponto de 0,17em na linha de base. **Só inicial maiúscula.** Champanhe é ornamento e nunca texto. |
| MayHouse | `assets/icone.svg` + `assets/css/style.css` | Primária é `#F6A821` (o `#E08700` era o tema claro do céu). Lilás `#8B7BD8`, janela acesa `#FFCF5E`, telhado `#4C3A52`. Display Baloo 2. |

**Três dos cinco proíbem caixa alta por escrito.** A planta 2D estava toda em
versalete e foi corrigida — rótulo de planta em caixa alta vira logotipo errado.

**Cor de marca é minoria em todos.** Carro do Freela pede 72% grafite e 8% ciano;
Pronta pede 60 superfície · 30 tinta · 10 marca. Por isso, no pavimento, a cor da
sala vive no **forro** — que é luz — e não em superfície grande.
