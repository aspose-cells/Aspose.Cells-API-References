---
title: "Class RadicalEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.RadicalEquationNode class. Denna klass specificerar radikalekvationen som består av en valfri grad degEquationNodeType.Degree och en bas"
type: docs
url: /sv/net/aspose.cells.drawing.equations/radicalequationnode/
---
## RadicalEquationNode class

Denna klass specificerar radikalekvationen, bestående av en valfri grad deg(EquationNodeType.Degree) och en bas.

```csharp
public class RadicalEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsDegHide](../../aspose.cells.drawing.equations/radicalequationnode/isdeghide/) { get; set; } | Om graden för radikaler ska döljas. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Anger föräldranoden för den aktuella noden (Ärvt från [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. (Ärvt från [`EquationNode`](../equationnode/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. (Ärvt från [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/radicalequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
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
    public class EquationsClassRadicalEquationNodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en textruta med ekvation i det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Lägg till en radikalekvationsnod
            RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            radicalNode.IsDegHide = true;

            // Lägg till grad (dold) och baskomponenter
            EquationNode degreeNode = radicalNode.AddChild(EquationNodeType.Degree);
            TextRunEquationNode degreeText = (TextRunEquationNode)degreeNode.AddChild(EquationNodeType.Text);
            degreeText.Text = "3";

            EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x + 1";

            // Spara arbetsboken
            workbook.Save("RadicalEquationDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera
            Workbook loadedWorkbook = new Workbook("RadicalEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            RadicalEquationNode loadedRadicalNode = (RadicalEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("Radical equation created successfully:");
            Console.WriteLine($"- IsDegHide: {loadedRadicalNode.IsDegHide}");
            Console.WriteLine($"- Base text: {((TextRunEquationNode)loadedRadicalNode.GetChild(1).GetChild(0)).Text}");
        }
    }
}
```

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


