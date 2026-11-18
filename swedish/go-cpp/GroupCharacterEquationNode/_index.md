---
title: "GroupCharacterEquationNode klass"
linktitle: "GroupCharacterEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "GroupCharacterEquationNode klass. Inkapslar objektet som representerar groupcharacterequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Denna klass specificerar Group‑Character‑funktionen, bestående av ett tecken som ritas ovanför eller under text, ofta för att visuellt gruppera objekt.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetGroupChr](./getgroupchr/) | Anger en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [SetGroupChr](./setgroupchr/) | Anger en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [GetChrType](./getchrtype/) | Specificera kombinerande tecken efter typvärde. |
| [SetChrType](./setchrtype/) | Specificera kombinerande tecken efter typvärde. |
| [GetPosition](./getposition/) | Detta attribut anger tecknets position i objektet |
| [SetPosition](./setposition/) | Detta attribut anger tecknets position i objektet |
| [GetVertJc](./getvertjc/) | Detta attribut, kombinerat med pos för groupChrPr, anger den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen. |
| [SetVertJc](./setvertjc/) | Detta attribut, kombinerat med pos för groupChrPr, anger den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Skapa en nod av den angivna typen. |
