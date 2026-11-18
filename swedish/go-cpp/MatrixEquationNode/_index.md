---
title: "MatrixEquationNode klass"
linktitle: "MatrixEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "MatrixEquationNode klass. Inkapslar objektet som representerar matrixequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Denna klass specificerar matrisekvationen, bestående av ett eller flera element ordnade i en eller flera rader och en eller flera kolumner.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetBaseJc](./getbasejc/) | Detta attribut anger justeringen av matrisen. Text utanför matrisen kan justeras med botten, toppen eller mitten av en matrisfunktion. Som standard antar matrisen centrerad justering. |
| [SetBaseJc](./setbasejc/) | Detta attribut anger justeringen av matrisen. Text utanför matrisen kan justeras med botten, toppen eller mitten av en matrisfunktion. Som standard antar matrisen centrerad justering. |
| [IsHidePlaceholder](./ishideplaceholder/) | Detta attribut specificerar egenskapen Hide Placeholders på en matris. När denna egenskap är på visas inte platshållare i matrisen. Som standard visas platshållare så att de platser där text kan infogas blir synliga. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Detta attribut specificerar egenskapen Hide Placeholders på en matris. När denna egenskap är på visas inte platshållare i matrisen. Som standard visas platshållare så att de platser där text kan infogas blir synliga. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Skapa en nod av den angivna typen. |
