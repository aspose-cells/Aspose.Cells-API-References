---
title: "Classe MatrixEquationNode"
linktitle: "MatrixEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe MatrixEquationNode. Incapsula l'oggetto che rappresenta matrixequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Questa classe specifica l'equazione Matrice, composta da uno o più elementi disposti in una o più righe e una o più colonne.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetBaseJc](./getbasejc/) | Questo attributo specifica l'allineamento della matrice. Il testo al di fuori della matrice può essere allineato in basso, in alto o al centro di una funzione matrice. Per impostazione predefinita, la matrice assume l'allineamento al centro. |
| [SetBaseJc](./setbasejc/) | Questo attributo specifica l'allineamento della matrice. Il testo al di fuori della matrice può essere allineato in basso, in alto o al centro di una funzione matrice. Per impostazione predefinita, la matrice assume l'allineamento al centro. |
| [IsHidePlaceholder](./ishideplaceholder/) | Questo attributo specifica la proprietà Nascondi Segnaposti su una matrice. Quando questa proprietà è attiva, i segnaposti non compaiono nella matrice. Per impostazione predefinita, i segnaposti compaiono in modo che le posizioni dove è possibile inserire testo siano visibili. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Questo attributo specifica la proprietà Nascondi Segnaposti su una matrice. Quando questa proprietà è attiva, i segnaposti non compaiono nella matrice. Per impostazione predefinita, i segnaposti compaiono in modo che le posizioni dove è possibile inserire testo siano visibili. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Crea un nodo del tipo specificato. |
