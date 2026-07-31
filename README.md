---
tipo: readme
data: 2026-07-31
produzido-por: Raphael Sousa Pizani Silva (OAB/BA 32.472)
versao-core: 1.0
---

# Auditor Estratégico Jurídico

> Skill para assistentes de IA. Audita o caso **antes** de qualquer redação —
> fatos, provas, teses, adversário, jurisprudência e riscos — e entrega dois
> documentos que nunca se misturam.

Peça bem escrita sobre material não auditado é o pior produto da advocacia: tem
aparência de solidez e não tem lastro. Esta skill trabalha antes disso. Ela não
redige — prepara o terreno para que a redação aconteça sobre material
classificado, hierarquizado e calibrado.

## Os dois produtos

| **Relatório Estratégico Interno** | **Dossiê de Redação** |
|---|---|
| Uso exclusivo do advogado | Insumo para a peça |
| "a testemunha é frágil" · "esse pedido existe para negociar" · "perdemos se o juízo seguir a linha X" | Só o que é processualmente aproveitável |
| Riscos, cenários, fraquezas, o que o cliente omitiu | Fatos com fonte, teses ordenadas, fundamentos, jurisprudência com status |

**A estanqueidade entre os dois é a regra mais importante da skill.** O teste de
admissão de cada parágrafo do Dossiê é: *"se este parágrafo caísse nos autos ou
chegasse ao adversário, causaria dano à parte?"* Se sim, não entra — sem exceção
e sem reformulação cosmética.

O que é estratégico só passa **traduzido em instrução neutra**:

> Interno: "a testemunha X é frágil e pode desmoronar."
> Dossiê: "não apoiar afirmação central exclusivamente no depoimento de X;
> ancorar nos documentos D1 e D3."

## Os nove módulos

A auditoria roda em silêncio e encadeada — cada módulo consome o produto do
anterior:

| | Módulo | Produto que entrega |
|---|---|---|
| **A** | Classificação de elementos | Quadro de Classificação: cada elemento como fato provado, fato alegado, inferência, tese ou opinião — com fonte apontável |
| **B** | Matriz probatória | fato × prova × ônus × status × providência. O vazio em fato essencial cujo ônus é nosso é o achado mais importante |
| **C** | Hierarquização argumentativa | Esqueleto: preliminares, principal, subsidiárias — e **a lista do que saiu, com o motivo** |
| **D** | Análise do adversário | Mapa do Adversário: contra-argumento provável e o mais perigoso, por tese |
| **E** | Argumento consequencialista | Blocos de reforço — ou o registro de que não há nenhum útil |
| **F** | Controle jurisprudencial | Quadro em três camadas: vinculante · persuasiva do tribunal competente · **contrária** |
| **G** | Calibração de confiança | Cada tese etiquetada N1 a N4, com o vocabulário que aquele nível autoriza |
| **H** | Consolidação multi-instância | O que nos vincula, o que precluiu, o alcance devolutivo do recurso |
| **I** | Riscos | Recursais, sucumbenciais e deontológicos — destino único: o Relatório |

## O módulo G: firmeza proporcional à solidez

A terceira premissa da skill é que **a firmeza do tom deve ser proporcional à
solidez da tese**. O módulo G a executa com uma tabela que liga condições
cumulativas a vocabulário permitido:

- **N1 sólida** — "é", "impõe-se", "não há como afastar";
- **N2 consistente** — "deve", "a orientação consolidada", "conclui-se". Proibido:
  "inequívoco", "cristalino", "pacífico";
- **N3 defensável** — "sustenta-se", "há fundamento para", "milita em favor".
  Proibido, além do anterior: advérbios de certeza e qualquer afirmação sobre o
  estado da jurisprudência;
- **N4 frágil** — apenas formulação subsidiária transparente ou pedido expresso
  de superação, apresentado como tal.

Rebaixar é sempre permitido; promover exige cumprir a condição, nunca o argumento
de necessidade ("precisamos soar firmes"). E quando o advogado discorda da
etiqueta — vai discordar, porque conhece o caso melhor —, a palavra final é dele:
a skill reetiqueta, registra a original e a razão, e não insiste.

## A terceira camada do módulo F

A camada mais importante é a que quase ninguém pesquisa: **a jurisprudência
contrária**. Encontrá-la antes do adversário é a diferença entre enfrentá-la nos
seus termos e ser surpreendido nos dele.

Se ela não foi pesquisada, a skill não finge que inexiste: registra a pendência,
**trava a calibração daquela tese no teto N3** por mais forte que pareça, entrega
o roteiro de busca, e proíbe no Dossiê qualquer afirmação sobre o estado da
jurisprudência. *Ausência de pesquisa nunca vira ausência de precedente
contrário.*

## Quando a informação não existe

É o estado normal do caso real, não a exceção. Nenhum módulo trava por falta de
dado: todos registram a lacuna com três atributos — o que falta, o que a falta
impede de concluir, qual providência a supre — e **rebaixam** qualquer conclusão
que dependia do dado ausente. Nunca se calibra pelo cenário otimista do que não
se sabe.

## Regimes

**Completo** (padrão, os nove módulos) · **Abreviado** (A, B, F e G, com a lista
expressa do que não foi auditado) · **Primeiro uso** (explica, entrega o
formulário e para) · **Não acionamento** (material que não é caso contencioso —
devolve o comando em uma frase).

## Escopo

Cobre contencioso cível, tributário, administrativo, empresarial, consumerista,
trabalhista, constitucional e penal econômico, com adaptações por matéria e por
posição processual (ativa, passiva, recursal).

Não cobre penal comum, família e sucessões, eleitoral e previdenciário
individual — nessas, avisa expressamente, roda em regime reduzido e marca os
produtos.

## Instalação

```bash
git clone https://github.com/pizaniadv/auditor-estrategico-juridico.git \
  ~/.claude/skills/auditor-estrategico-juridico
```

Skills seguem o padrão aberto [Agent Skills](https://agentskills.io) — o
`SKILL.md` funciona em outras ferramentas compatíveis. A skill é autossuficiente:
não depende de outro arquivo, base de dados ou ferramenta.

## Como usar

`/auditor-estrategico-juridico`, ou: "audite este caso" · "antes de redigir,
audite" · "relatório estratégico" · "avalie as teses antes da peça".

## O que ela não faz

Não promete êxito, não estima "chance de vitória" em número, não decide pelo
advogado e não substitui o exame direto dos autos. Não cita julgado de memória —
descreve a orientação em tese e entrega o roteiro de busca. E não redige sem
comando expresso; quando redige, a única fonte é o Dossiê.

## Família

Complementos opcionais — esta skill executa sozinha:
[`antialucinacao-juridica`](https://github.com/pizaniadv/antialucinacao-juridica) ·
[`inferencia-jurisprudencial-mij`](https://github.com/pizaniadv/inferencia-jurisprudencial-mij) ·
[`critica-adversarial-juridica`](https://github.com/pizaniadv/critica-adversarial-juridica) ·
[`validacao-logica-forense`](https://github.com/pizaniadv/validacao-logica-forense) ·
[`verificar-lendo-a-fonte`](https://github.com/pizaniadv/verificar-lendo-a-fonte) ·
[`revisao-que-sugere`](https://github.com/pizaniadv/revisao-que-sugere) ·
[`ritual-de-encerramento`](https://github.com/pizaniadv/ritual-de-encerramento) ·
[`handoff-de-sessao`](https://github.com/pizaniadv/handoff-de-sessao).

## Licença

A partir da versão 2.0.0, licenciamento duplo, ambos copyleft, ambos com
**atribuição nominal obrigatória**: **[AGPL-3.0](LICENSE)** para o componente
executável e **[CC BY-SA 4.0](LICENSE-DOCS)** para a obra textual.

Uso no seu escritório não gera obrigação nenhuma. **Distribuir** versão
modificada, ou **oferecê-la a terceiros como serviço**, exige abrir o código e
manter a atribuição. O [NOTICE](NOTICE) é parte da licença.

A versão 1.0.0, publicada em abril de 2026, foi distribuída sob CC BY 4.0 e
permanece disponível sob aquela licença no histórico do repositório — licença
concedida não se revoga.

## Autor

**Raphael Sousa Pizani Silva** — OAB/BA 32.472
[github.com/pizaniadv](https://github.com/pizaniadv)

Histórico de versões no [CHANGELOG](CHANGELOG.md).
