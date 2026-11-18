---
title: "DelimiterEquationNode-klass"
linktitle: "DelimiterEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DelimiterEquationNode-klass. Inkapslar objektet som representerar delimiterequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Denna klass specificerar avgränsarekvationen, bestående av öppnings- och stängningsavgränsare (såsom parenteser, klammerparenteser, hakparenteser och vertikala streck) samt en komponent som finns inuti. Avgränsaren kan ha mer än en komponent, med ett bestämt separator‑tecken mellan varje komponent.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetBeginChar](./getbeginchar/) | Avgränsningens starttecken. |
| [SetBeginChar](./setbeginchar/) | Avgränsningens starttecken. |
| [GetEndChar](./getendchar/) | Avgränsningens sluttecken. |
| [SetEndChar](./setendchar/) | Avgränsningens sluttecken. |
| [GetNaryGrow](./getnarygrow/) | Anger om avgränsningen automatiskt ska expandera och kontrahera med formelns höjd. |
| [SetNaryGrow](./setnarygrow/) | Anger om avgränsningen automatiskt ska expandera och kontrahera med formelns höjd. |
| [GetSeparatorChar](./getseparatorchar/) | Avgränsningsseparatortecken. |
| [SetSeparatorChar](./setseparatorchar/) | Avgränsningsseparatortecken. |
| [GetDelimiterShape](./getdelimitershape/) | Anger formen på avgränsningarna i avgränsningsobjektet. |
| [SetDelimiterShape](./setdelimitershape/) | Anger formen på avgränsningarna i avgränsningsobjektet. |
| [Equals](./equals/) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [GetStartIndex](./getstartindex/) | Hämtar startindexet för tecknen. |
| [GetLength](./getlength/) | Hämtar längden på tecknen. |
| [GetFont](./getfont/) | Returnerar teckensnittet för detta objekt. |
| [SetWordArtStyle](./setwordartstyle/) | Ställer in den förinställda WordArt-stilen. |
| [GetTextOptions](./gettextoptions/) | Returnerar textalternativen. |
| [GetType](./gettype/) | Hämtar typen av textnod. |
| [GetParentNode](./getparentnode/) | Anger föräldranoden för den aktuella noden |
| [SetParentNode](./setparentnode/) | Anger föräldranoden för den aktuella noden |
| [ToLaTeX](./tolatex/) | Konvertera denna ekvation till ett LaTeX-uttryck. |
| [ToMathML](./tomathml/) | Konvertera denna ekvation till ett MathML-uttryck. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Infoga en nod av den angivna typen i slutet av listan med barnnoder för den aktuella noden. |
| [InsertChild](./insertchild/) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens lista med barnnoder. |
| [InsertAfter](./insertafter/) | Infogar den angivna noden efter den aktuella noden. |
| [InsertBefore](./insertbefore/) | Infogar den angivna noden före den aktuella noden. |
| [GetChild](./getchild/) | Returnerar noden på det angivna indexet bland barnen till den aktuella noden. |
| [Remove](./remove/) | Tar bort sig själv från föräldern. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Tar bort den angivna noden från den aktuella nodens barn. |
| [RemoveAllChildren](./removeallchildren/) | Tar bort alla barnnoder från den aktuella noden. |
| [GetEquationType](./getequationtype/) | Hämta ekvationstypen för den aktuella noden |
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Skapa en nod av den angivna typen. |
