---
title: "Classe AccentEquationNode"
linktitle: "AccentEquationNode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe AccentEquationNode. Incapsula l'oggetto che rappresenta accentequationnode in Go."
type: docs
weight: 200
url: /it/go-cpp/accentequationnode/
---

## AccentEquationNode class

Questa classe specifica un'equazione di accento, composta da un componente base e un diacritico combinante.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetAccentCharacter](./getaccentcharacter/) | Questo attributo specifica il tipo di segno diacritico combinante collegato alla base della funzione di accento. Il carattere di accento predefinito è U+0302. Si consiglia vivamente di utilizzare l'attributo AccentType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo conosciuto. |
| [SetAccentCharacter](./setaccentcharacter/) | Questo attributo specifica il tipo di segno diacritico combinante collegato alla base della funzione di accento. Il carattere di accento predefinito è U+0302. Si consiglia vivamente di utilizzare l'attributo AccentType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo conosciuto. |
| [GetAccentCharacterType](./getaccentcharactertype/) | Specifica i caratteri combinanti per valore di tipo. |
| [SetAccentCharacterType](./setaccentcharactertype/) | Specifica i caratteri combinanti per valore di tipo. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | Crea un nodo del tipo specificato. |
