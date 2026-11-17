---
title: "Classe DelimiterEquationNode"
linktitle: "DelimiterEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe DelimiterEquationNode. Incapsula l'oggetto che rappresenta delimiterequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Questa classe specifica l'equazione delimitatore, composta da delimitatori di apertura e chiusura (come parentesi tonde, graffe, parentesi quadre e barre verticali) e da un componente contenuto all'interno. Il delimitatore può avere più di un componente, con un carattere separatore designato tra ciascun componente.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetBeginChar](./getbeginchar/) | Carattere di inizio delimitatore. |
| [SetBeginChar](./setbeginchar/) | Carattere di inizio delimitatore. |
| [GetEndChar](./getendchar/) | Carattere di fine delimitatore. |
| [SetEndChar](./setendchar/) | Carattere di fine delimitatore. |
| [GetNaryGrow](./getnarygrow/) | Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula. |
| [SetNaryGrow](./setnarygrow/) | Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula. |
| [GetSeparatorChar](./getseparatorchar/) | Carattere separatore del delimitatore. |
| [SetSeparatorChar](./setseparatorchar/) | Carattere separatore del delimitatore. |
| [GetDelimiterShape](./getdelimitershape/) | Specifica la forma dei delimitatori nell'oggetto delimitatore. |
| [SetDelimiterShape](./setdelimitershape/) | Specifica la forma dei delimitatori nell'oggetto delimitatore. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Crea un nodo del tipo specificato. |
