---
title: "Klass MatrixEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.MatrixEquationNode klass. Denna klass specificerar Matrix-ekvationen som består av ett eller flera element placerade i en eller flera rader och en eller flera kolumner"
type: docs
url: /sv/net/aspose.cells.drawing.equations/matrixequationnode/
---
## MatrixEquationNode class

Denna klass specificerar Matrix‑ekvationen, bestående av ett eller flera element arrangerade i en eller flera rader och en eller flera kolumner.

```csharp
public class MatrixEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BaseJc](../../aspose.cells.drawing.equations/matrixequationnode/basejc/) { get; set; } | Detta attribut specificerar justeringen av matrisen. Text utanför matrisen kan justeras med botten, toppen eller mitten av en matrisfunktion. Som standard antar matrisen centrerad justering. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHidePlaceholder](../../aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/) { get; set; } | Detta attribut specificerar egenskapen Hide Placeholders på en matris. När denna egenskap är aktiverad visas inte platshållare i matrisen. Som standard visas platshållare så att de platser där text kan infogas blir synliga. |
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
| override [Equals](../../aspose.cells.drawing.equations/matrixequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
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
    public class EquationsClassMatrixEquationNodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en textruta med ekvation i det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationstycket och lägg till en matrisnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Ställ in matrisens egenskaper
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Lägg till en 2x2-matris med 1:or på diagonalen
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Spara arbetsboken
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);
            Console.WriteLine("Matrix equation created successfully. File saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


