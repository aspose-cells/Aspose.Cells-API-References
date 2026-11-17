---
title: "FractionEquationNode Classe"
linktitle: "FractionEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "FractionEquationNode classe. Incapsula l'oggetto che rappresenta fractionequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/fractionequationnode/
---

## FractionEquationNode class

Questa classe specifica l'equazione frazione, composta da un numeratore e un denominatore separati da una barra di frazione. La barra di frazione può essere orizzontale o diagonale, a seconda delle proprietà della frazione. L'equazione frazione è anche usata per rappresentare la funzione stack, che posiziona un elemento sopra un altro, senza barra di frazione.

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetFractionType](./getfractiontype/) | Questo specifica il tipo di frazione ; il valore predefinito è 'Bar'. |
| [SetFractionType](./setfractiontype/) | Questo specifica il tipo di frazione ; il valore predefinito è 'Bar'. |
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
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | Crea un nodo del tipo specificato. |
