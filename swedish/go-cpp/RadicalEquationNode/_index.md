---
title: "RadicalEquationNode klass"
linktitle: "RadicalEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "RadicalEquationNode klass. Inkapslar objektet som representerar radicalequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/radicalequationnode/
---

## RadicalEquationNode class

Denna klass specificerar radikekvationen, bestående av en valfri grad deg(EquationNodeType.Degree) och en bas.

```go

type RadicalEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewRadicalEquationNode](./newradicalequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsDegHide](./isdeghide/) | Om graden av radikaler ska döljas. |
| [SetIsDegHide](./setisdeghide/) | Om graden av radikaler ska döljas. |
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
| [RadicalEquationNode_CreateNode](./radicalequationnode_createnode/) | Skapa en nod av den angivna typen. |
