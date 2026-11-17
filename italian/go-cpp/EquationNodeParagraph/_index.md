---
title: "Classe EquationNodeParagraph"
linktitle: "EquationNodeParagraph"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe EquationNodeParagraph. Incapsula l'oggetto che rappresenta equationnodeparagraph in Go."
type: docs
weight: 200
url: /it/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

Questa classe specifica un paragrafo matematico contenente uno o più elementi MathEquationNode(OMath).

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetJustification](./getjustification/) | Specifica l'allineamento del paragrafo matematico (una serie di equazioni adiacenti nello stesso paragrafo). Un paragrafo matematico può essere allineato a sinistra, allineato a destra, centrato o centrato come gruppo. Per impostazione predefinita, il paragrafo matematico è centrato come gruppo. Ciò significa che le equazioni possono essere allineate tra loro, ma l'intero gruppo di equazioni è centrato nel suo insieme. |
| [SetJustification](./setjustification/) | Specifica l'allineamento del paragrafo matematico (una serie di equazioni adiacenti nello stesso paragrafo). Un paragrafo matematico può essere allineato a sinistra, allineato a destra, centrato o centrato come gruppo. Per impostazione predefinita, il paragrafo matematico è centrato come gruppo. Ciò significa che le equazioni possono essere allineate tra loro, ma l'intero gruppo di equazioni è centrato nel suo insieme. |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Crea un nodo del tipo specificato. |
