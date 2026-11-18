---
title: "NaryEquationNode klass"
linktitle: "NaryEquationNode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "NaryEquationNode-klass. Inkapslar objektet som representerar naryequationnode i Go."
type: docs
weight: 200
url: /sv/go-cpp/naryequationnode/
---

## NaryEquationNode class

Denna klass specificerar en n‑är operator‑ekvation bestående av en n‑är operator, en bas (eller operand) samt valfria övre och nedre gränser.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsHideSubscript](./ishidesubscript/) | Om den nedre gränsen ska visas |
| [SetIsHideSubscript](./setishidesubscript/) | Om den nedre gränsen ska visas |
| [IsHideSuperscript](./ishidesuperscript/) | Om den övre gränsen ska visas |
| [SetIsHideSuperscript](./setishidesuperscript/) | Om den övre gränsen ska visas |
| [GetLimitLocation](./getlimitlocation/) | Detta attribut anger placeringen av gränser i n-ära operatorer. Gränser kan antingen vara centrerade ovanför och under den n-ära operatorn, eller placerade precis till höger om operatorn. |
| [SetLimitLocation](./setlimitlocation/) | Detta attribut anger placeringen av gränser i n-ära operatorer. Gränser kan antingen vara centrerade ovanför och under den n-ära operatorn, eller placerade precis till höger om operatorn. |
| [GetNaryOperator](./getnaryoperator/) | en n-är operator.t.ex. "∑". Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [SetNaryOperator](./setnaryoperator/) | en n-är operator.t.ex. "∑". Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ. |
| [GetNaryOperatorType](./getnaryoperatortype/) | en n-är operator.t.ex. "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | en n-är operator.t.ex. "∑" |
| [GetNaryGrow](./getnarygrow/) | Detta attribut anger tillväxtsegenskapen för n-ära operatorer på dokumentnivå. När den är avstängd växer n-ära operatorer såsom integraler och summor inte för att matcha operandens höjd. När den är påslagen växer den n-ära operatorn vertikalt för att matcha operandens höjd. |
| [SetNaryGrow](./setnarygrow/) | Detta attribut anger tillväxtsegenskapen för n-ära operatorer på dokumentnivå. När den är avstängd växer n-ära operatorer såsom integraler och summor inte för att matcha operandens höjd. När den är påslagen växer den n-ära operatorn vertikalt för att matcha operandens höjd. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Skapa en nod av den angivna typen. |
