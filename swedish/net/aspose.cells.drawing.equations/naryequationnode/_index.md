---
title: "Klass NaryEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode-klass. Denna klass specificerar en n-är operator-ekvation som består av en n-är operator, en bas eller operand och valfria övre och nedre gränser."
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

Denna klass specificerar en n‑är operator‑ekvation bestående av en n‑är operator, en bas (eller operand) samt valfria övre och nedre gränser.

```csharp
public class NaryEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | Om den nedre gränsen ska visas |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | Om den övre gränsen ska visas |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | Detta attribut anger placeringen av gränser i n-ära operatorer. Gränser kan antingen vara centrerade ovanför och under den n-ära operatorn, eller placerade precis till höger om operatorn. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | Detta attribut anger tillväxtegenskapen för n-ära operatorer på dokumentnivå. När den är av, växer n-ära operatorer såsom integraler och summor inte för att matcha operandens höjd. När den är på, växer den n-ära operatorn vertikalt för att matcha operandens höjd. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | en n-är operator.t.ex \"∑\". Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd denna egenskapsinställning om du inte kan hitta tecknet du behöver i en känd typ. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | en n-är operator.t.ex \"∑\" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Anger föräldranoden för den aktuella noden (Ärvt från [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. (Ärvt från [`EquationNode`](../equationnode/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. (Ärvt från [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
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
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en n-är ekvationsnod
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Ställ in n-ära egenskaper
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // Lägg till baskomponent
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // Spara arbetsboken
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


