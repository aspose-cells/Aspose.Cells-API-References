---
title: "TextBox.GetEquationParagraph"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBox‑metod. Hämtar det angivna matematiska stycket från TextBody‑egenskapen i TextBox‑objektet. Observera 1 Returnerar NULL när indexet är utanför gränserna eller inte hittas. 2 Returnerar också NULL om den angivna indexpositionen inte är ett matematiskt stycke."
type: docs
url: /sv/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Hämta det angivna matematiska stycket från TextBody-egenskapen i TextBox-objektet. Observera: (1) Returnerar NULL när indexet är utanför gränserna eller inte hittas. (2) Returnerar också NULL om den angivna indexpositionen inte är ett matematiskt stycke.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Positionsindexet för den matematiska paragrafen, med början från 0. |

### Returvärde

Returnerar den matematiska paragrafen som anges av indexet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class TextBoxMethodGetEquationParagraphWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i arbetsbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Lägg till lite ekvationsinnehåll i textrutan
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Anropa GetEquationParagraph med indexparameter (Int32)
                EquationNode equationNode = textBox.GetEquationParagraph(0);

                if (equationNode != null)
                {
                    Console.WriteLine("Equation paragraph retrieved successfully.");
                    Console.WriteLine($"Equation type: {equationNode.EquationType}");
                    Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
                }
                else
                {
                    Console.WriteLine("No equation paragraph found at the specified index.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Hämtar det första matematiska stycket från TextBody-egenskapen i TextBox-objektet.

```csharp
public EquationNode GetEquationParagraph()
```

### Returvärde

Om det finns en matematisk paragraf, returneras den första, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextBoxMethodGetEquationParagraphDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "$$\\sqrt{x^2+y^2}$$";
            
            EquationNode equationNode = textBox.GetEquationParagraph();
            
            if (equationNode != null)
            {
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
            }
            else
            {
                Console.WriteLine("No equation paragraph found");
            }
        }
    }
}
```

### Se även

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


