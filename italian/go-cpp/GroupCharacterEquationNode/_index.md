---
title: "Classe GroupCharacterEquationNode"
linktitle: "GroupCharacterEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe GroupCharacterEquationNode. Incapsula l'oggetto che rappresenta groupcharacterequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Questa classe specifica la funzione Group-Character, composta da un carattere disegnato sopra o sotto il testo, spesso con lo scopo di raggruppare visivamente gli elementi.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetGroupChr](./getgroupchr/) | Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto. |
| [SetGroupChr](./setgroupchr/) | Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto. |
| [GetChrType](./getchrtype/) | Specifica i caratteri combinanti per valore di tipo. |
| [SetChrType](./setchrtype/) | Specifica i caratteri combinanti per valore di tipo. |
| [GetPosition](./getposition/) | Questo attributo specifica la posizione del carattere nell'oggetto |
| [SetPosition](./setposition/) | Questo attributo specifica la posizione del carattere nell'oggetto |
| [GetVertJc](./getvertjc/) | Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. Dove pos indica la posizione del carattere di raggruppamento, vertJc specifica l'allineamento dell'oggetto rispetto alla linea di base. |
| [SetVertJc](./setvertjc/) | Questo attributo, combinato con pos di groupChrPr, specifica il layout verticale dell'oggetto groupChr. Dove pos indica la posizione del carattere di raggruppamento, vertJc specifica l'allineamento dell'oggetto rispetto alla linea di base. |
| [Equals](./equals/) | Determina se il nodo equazione corrente è uguale al nodo specificato |
| [GetStartIndex](./getstartindex/) | Ottiene l'indice iniziale dei caratteri. |
| [GetLength](./getlength/) | Ottiene la lunghezza dei caratteri. |
| [GetFont](./getfont/) | Restituisce il font di questo oggetto. |
| [SetWordArtStyle](./setwordartstyle/) | Imposta lo stile WordArt predefinito. |
| [GetTextOptions](./gettextoptions/) | Restituisce le opzioni di testo. |
| [GetType](./gettype/) | Ottiene il tipo di nodo di testo. |
| [GetParentNode](./getparentnode/) | Specifica il nodo genitore del nodo corrente |
| [SetParentNode](./setparentnode/) | Specifica il nodo genitore del nodo corrente |
| [ToLaTeX](./tolatex/) | Converti questa equazione in un'espressione LaTeX. |
| [ToMathML](./tomathml/) | Converti questa equazione in un'espressione MathML. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente. |
| [InsertChild](./insertchild/) | Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente. |
| [InsertAfter](./insertafter/) | Inserisce il nodo specificato dopo il nodo corrente. |
| [InsertBefore](./insertbefore/) | Inserisce il nodo specificato prima del nodo corrente. |
| [GetChild](./getchild/) | Restituisce il nodo all'indice specificato tra i figli del nodo corrente. |
| [Remove](./remove/) | Rimuove se stesso dal genitore. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Rimuove il nodo specificato dai figli del nodo corrente. |
| [RemoveAllChildren](./removeallchildren/) | Rimuove tutti i nodi figlio del nodo corrente. |
| [GetEquationType](./getequationtype/) | Ottieni il tipo di equazione del nodo corrente |
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Crea un nodo del tipo specificato. |
