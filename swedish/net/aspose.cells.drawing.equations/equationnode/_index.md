---
title: "Klass EquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationNode-klass. Abstrakt klass för att härleda andra ekvationsnoder"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class

Abstrakt klass för att härleda andra ekvationsnoder.

```csharp
public abstract class EquationNode : FontSetting
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specificerar föräldranoden för den aktuella noden |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [CreateNode](../../aspose.cells.drawing.equations/equationnode/createnode/)(EquationNodeType, Workbook, EquationNode) | Skapa en nod av den angivna typen. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild_1)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/#addchild)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. |
| override [Equals](../../aspose.cells.drawing.equations/equationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returnerar noden på det angivna indexet bland den aktuella nodens barn. |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Infogar den angivna noden efter den aktuella noden. |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Infogar den angivna noden före den aktuella noden. |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens lista över barnnoder. |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Tar bort sig själv från föräldern. |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Tar bort alla barnnoder för den aktuella noden. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild)(EquationNode) | Tar bort den angivna noden från den aktuella nodens barn. |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/#removechild_1)(int) | Tar bort noden på det angivna indexet från den aktuella nodens barn. |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt‑stilen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Konvertera denna ekvation till LaTeX-uttryck. |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Konvertera denna ekvation till MathML-uttryck. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta i kalkylbladet och hämta dess index.
            int textBoxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "=A1+B1";
            
            // Hämta ekvationsnoden från textrutan.
            EquationNode node = textBox.GetEquationParagraph();
            
            // Skriv ut ekvationstexten med ToString().
            Console.WriteLine("Equation: " + node.ToString());
            
            // Modifiera ekvationen genom att ange ny text.
            textBox.Text = "=A1*B1";
            Console.WriteLine("Modified Equation: " + textBox.Text);
        }
    }
}
```

### Se även

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


