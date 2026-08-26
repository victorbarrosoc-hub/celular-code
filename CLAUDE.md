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

# Briefing em aberto — NÃO EXECUTAR ATÉ LIBERAÇÃO

> Registrado em 26/08/2026. O Victor pediu explicitamente para **armazenar e não
> fazer nada** até ele dizer que pode. Quando ele liberar, é este o programa.

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
| Espaço de convívio | de uso mútuo do HUB, comum aos cinco produtos |
| Local de despressurização | descompressão, descanso |
| Copa | para café |
| Local para almoço | refeição |

Somados às sete salas já desenhadas (cinco de produto + duas de reunião,
*Marca* e *Máquina*), o pavimento passa a ter área social além da área de
trabalho.

**4 · Liberdade criativa autorizada.** "Enfim, seja criativo."

## Referências

Virão por anexo do Victor. Guardar em [`referencias/`](referencias/LEIA.md) e
anotar ali o que cada uma traz. **Até o momento não chegou nenhuma** — na
mensagem em que ele as citou, os anexos não vieram.

## Perguntas a resolver quando liberar

- A demonstração em imagem substitui a planta baixa atual ou convive com ela?
  (A planta carrega a regra "área = quanto de produto existe", que hoje é o
  raciocínio central da página — perder isso tem custo.)
- Ponto de vista: uma vista por sala, ou um percurso contínuo pelo pavimento?
- Os ambientes sociais entram na planta com a mesma neutralidade das salas de
  reunião — sem cor de dono, janela dividida nos cinco tons?
