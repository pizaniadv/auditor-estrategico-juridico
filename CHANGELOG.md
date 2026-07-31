# Changelog

Todas as alteracoes relevantes deste projeto sao documentadas neste arquivo.

O formato segue [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e o
versionamento adota [Semantic Versioning](https://semver.org/lang/pt-BR/).

---

## [2.0.0] — 2026-07-31

### Reescrita integral

A skill foi **reescrita do zero**. A versao anterior era um delta: remetia oito
vezes a uma "V1 universal" que nunca foi publicada e nao existia em arquivo
nenhum. Sete secoes diziam "identico a V1" e estavam vazias — os nove modulos de
auditoria, os itens do Relatorio e os do Dossie simplesmente nao constavam do
pacote. Instalada, a skill nao rodava por inteiro, e foi assim que um usuario a
recebeu.

Esta versao nao remenda aquele delta nem tenta reconstituir a V1 perdida: e obra
nova, completa e autossuficiente, que ocupa o mesmo nome.

### Adicionado

- Os **nove modulos A–I**, escritos por inteiro. Cada um com as perguntas que faz
  ao material, o criterio que separa resposta boa de ruim, o produto que entrega
  ao modulo seguinte, e a regra para quando a informacao nao existe.
- **Regra de estanqueidade** entre os dois produtos, com teste de admissao por
  paragrafo ("se este paragrafo caisse nos autos, causaria dano?"), lista de
  bloqueio de termos e padrao de traducao de conteudo interno em instrucao
  neutra de redacao.
- **Escala N1–N4 do modulo G**, ligando condicoes cumulativas ao vocabulario
  autorizado e proibido em cada nivel — o mecanismo que executa a premissa de que
  a firmeza do tom e proporcional a solidez da tese.
- **Regra da camada 3 do modulo F**: jurisprudencia contraria nao pesquisada
  registra pendencia, trava a calibragem no teto N3, gera roteiro de busca e
  proibe afirmacao sobre o estado da jurisprudencia no Dossie. Ausencia de
  pesquisa nunca vira ausencia de precedente contrario.
- **Regra transversal de informacao faltante**: nenhum modulo trava por falta de
  dado; todos registram a lacuna com tres atributos e rebaixam a conclusao que
  dela dependia.
- **Sobreposicao pelo advogado**: quando ele discorda da etiqueta de calibragem,
  a palavra final e dele — a skill reetiqueta, registra a original com a razao, e
  nao insiste.
- Adaptacoes por seis materias e por tres posicoes processuais; checklist final
  bloqueante; onboarding com instalacao, alimentacao, leitura e iteracao.

### Alterado

- **Licenciamento.** A partir desta versao: AGPL-3.0 (componente executavel) +
  CC BY-SA 4.0 (obra textual), com termo adicional de atribuicao pelo art. 7(b)
  da AGPL, alinhando esta skill a familia publicada em 30/07/2026. A versao 1.0.0
  foi distribuida sob CC BY 4.0 e permanece disponivel sob aquela licenca no
  historico do repositorio — licenca concedida nao se revoga.
- Rigor de citacao: apenas dispositivos notorios, com o teor conferido; institutos
  descritos sem numero onde havia duvida; zero julgados, sumulas ou temas citados.

### Removido

- Toda remissao a conteudo externo ao arquivo. A skill nao depende de versao
  anterior, de skill irma nem de base de dados.
- O aviso de incompletude que constava do README desde 30/07/2026, agora sem
  objeto.

---

## [1.0.0] — 2026-04-23

- Versao inicial da skill.
- Nove modulos de auditoria; tres regimes de operacao; adaptacoes por materia e
  por posicao processual; protocolo antialucinatorio; separacao entre Relatorio
  Estrategico Interno e Dossie de Redacao.
- Licenciada sob Creative Commons Attribution 4.0 International (CC BY 4.0).

> Nota historica: o arquivo `SKILL.md` efetivamente publicado nesta versao era a
> V2 (um delta sobre a V1), e nao a versao que este registro descreve. A
> divergencia so foi detectada em 30/07/2026, quando a skill foi instalada por um
> terceiro. Ver a versao 2.0.0.
