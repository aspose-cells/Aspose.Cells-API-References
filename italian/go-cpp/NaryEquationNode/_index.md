---
title: "NaryEquationNode Classe"
linktitle: "NaryEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe NaryEquationNode. Incapsula l'oggetto che rappresenta naryequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/naryequationnode/
---

## NaryEquationNode class

Questa classe specifica un'equazione di operatore n-ario composta da un operatore n-ario, una base (o operando) e limiti superiori e inferiori opzionali.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsHideSubscript](./ishidesubscript/) | Se visualizzare il limite inferiore |
| [SetIsHideSubscript](./setishidesubscript/) | Se visualizzare il limite inferiore |
| [IsHideSuperscript](./ishidesuperscript/) | Se visualizzare il limite superiore |
| [SetIsHideSuperscript](./setishidesuperscript/) | Se visualizzare il limite superiore |
| [GetLimitLocation](./getlimitlocation/) | Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore. |
| [SetLimitLocation](./setlimitlocation/) | Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore. |
| [GetNaryOperator](./getnaryoperator/) | un operatore n-ario, ad es. "∑". È fortemente consigliato utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto. |
| [SetNaryOperator](./setnaryoperator/) | un operatore n-ario, ad es. "∑". È fortemente consigliato utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto. |
| [GetNaryOperatorType](./getnaryoperatortype/) | un operatore n-ario, ad es. "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | un operatore n-ario, ad es. "∑" |
| [GetNaryGrow](./getnarygrow/) | Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando è disattivato, gli operatori n-ari come integrali e sommatorie non crescono per corrispondere all'altezza del loro operando. Quando è attivato, l'operatore n-ario cresce verticalmente per corrispondere all'altezza del suo operando. |
| [SetNaryGrow](./setnarygrow/) | Questo attributo specifica la proprietà di crescita degli operatori n-ari a livello di documento. Quando è disattivato, gli operatori n-ari come integrali e sommatorie non crescono per corrispondere all'altezza del loro operando. Quando è attivato, l'operatore n-ario cresce verticalmente per corrispondere all'altezza del suo operando. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Crea un nodo del tipo specificato. |
