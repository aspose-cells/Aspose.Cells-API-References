---
title: "TextBox.GetEquationParagraph"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBox-Methode. Gibt den angegebenen mathematischen Absatz aus der TextBody-Eigenschaft des TextBox-Objekts zurück. Hinweis 1 Gibt NULL zurück, wenn der Index außerhalb des Bereichs liegt oder nicht gefunden wird. 2 Gibt ebenfalls NULL zurück, wenn die angegebene Indexposition kein mathematischer Absatz ist."
type: docs
url: /de/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Ruft den angegebenen mathematischen Absatz aus der TextBody-Eigenschaft des TextBox-Objekts ab. Hinweis: (1) Gibt NULL zurück, wenn der Index außerhalb des Bereichs liegt oder nicht gefunden wird. (2) Gibt ebenfalls NULL zurück, wenn die angegebene Indexposition kein mathematischer Absatz ist.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Positionsindex des mathematischen Absatzes, beginnend bei 0. |

### Rückgabewert

Gibt den durch den Index angegebenen mathematischen Absatz zurück.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Fügen Sie dem Textfeld etwas Gleichungsinhalt hinzu
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Rufen Sie GetEquationParagraph mit dem Indexparameter (Int32) auf
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

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Liefert den ersten mathematischen Absatz aus der TextBody-Eigenschaft des TextBox-Objekts.

```csharp
public EquationNode GetEquationParagraph()
```

### Rückgabewert

Falls ein mathematischer Absatz vorhanden ist, wird der erste zurückgegeben, andernfalls wird null zurückgegeben.

### Beispiele

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

### Siehe auch

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


