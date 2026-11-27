---
title: "Class GroupCharacterEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.GroupCharacterEquationNode klass. Denna klass specificerar GroupCharacter-funktionen som består av ett tecken ritat ovanför eller under text, ofta i syfte att visuellt gruppera objekt"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/
---
## GroupCharacterEquationNode class

Denna klass specificerar Group-Character‑funktionen, bestående av ett tecken som ritas ovanför eller under text, ofta för att visuellt gruppera objekt.

```csharp
public class GroupCharacterEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ChrType](../../aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/) { get; set; } | Specificera kombinerande tecken med typvärde. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [GroupChr](../../aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/) { get; set; } | Anger en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd denna egenskapsinställning om du inte kan hitta tecknet du behöver i en känd typ. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Anger föräldranoden för den aktuella noden (Ärvt från [`EquationNode`](../equationnode/).) |
| [Position](../../aspose.cells.drawing.equations/groupcharacterequationnode/position/) { get; set; } | Detta attribut anger tecknets position i objektet |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. (Ärvt från [`EquationNode`](../equationnode/).) |
| [VertJc](../../aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/) { get; set; } | Detta attribut, kombinerat med pos för groupChrPr, anger den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. (Ärvt från [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/groupcharacterequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returnerar noden på det angivna indexet bland den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Infogar den angivna noden efter den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Infogar den angivna noden före den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista. (Ärvt från [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Tar bort sig själv från föräldern. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Tar bort alla barnnoder för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Tar bort den angivna noden från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Tar bort noden på det angivna indexet från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt‑stilen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Konvertera denna ekvation till ett LaTeX‑uttryck. (Ärvt från [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Konvertera denna ekvation till MathML-uttryck.(Härledd från [`EquationNode`](../equationnode/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassGroupCharacterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Hämta matematiknod och lägg till grupperingstecken
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupCharNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Konfigurera egenskaper för grupperingstecken
            groupCharNode.Position = EquationCharacterPositionType.Top;
            groupCharNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
            
            // Lägg till bastext
            EquationNode baseNode = groupCharNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";
            
            // Spara arbetsboken
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


