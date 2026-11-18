---
title: "AccentEquationNode-klass"
linktitle: "AccentEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AccentEquationNode-klass. Inkapslar objektet som representerar accentequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/accentequationnode/
---

## AccentEquationNode class

Denna klass specificerar en accentekvation, bestående av en baskomponent och en kombinerande diakritisk markering.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetAccentCharacter](./getaccentcharacter/) | Detta attribut anger typen av kombinerande diakritisk markering som är fäst vid basen för accentfunktionen. Standardaccenttecknet är U+0302. Det rekommenderas starkt att använda attributet AccentType för att ange accenttecken. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [SetAccentCharacter](./setaccentcharacter/) | Detta attribut anger typen av kombinerande diakritisk markering som är fäst vid basen för accentfunktionen. Standardaccenttecknet är U+0302. Det rekommenderas starkt att använda attributet AccentType för att ange accenttecken. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [GetAccentCharacterType](./getaccentcharactertype/) | Specificera kombinerande tecken efter typvärde. |
| [SetAccentCharacterType](./setaccentcharactertype/) | Specificera kombinerande tecken efter typvärde. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | Skapa en nod av den angivna typen. |
