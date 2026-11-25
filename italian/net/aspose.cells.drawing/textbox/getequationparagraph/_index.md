---
title: "TextBox.GetEquationParagraph"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextBox. Ottieni il paragrafo matematico specificato dalla proprietà TextBody dell'oggetto TextBox. Nota 1 Restituisce NULL quando l'indice è fuori dai limiti o non trovato. 2 Restituisce anche NULL se la posizione dell'indice specificato non è un paragrafo matematico"
type: docs
url: /it/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Ottieni il paragrafo matematico specificato dalla proprietà TextBody dell'oggetto TextBox. Nota: (1) Restituisce NULL quando l'indice è fuori dai limiti o non trovato. (2) Restituisce anche NULL se la posizione dell'indice specificato non è un paragrafo matematico.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice di posizione del paragrafo matematico, a partire da 0. |

### Valore di ritorno

Restituisce il paragrafo matematico specificato dall'indice.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Aggiungi del contenuto di equazione alla casella di testo
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Chiama GetEquationParagraph con il parametro indice (Int32)
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

            // Salva la cartella di lavoro
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Ottiene il primo paragrafo matematico dalla proprietà TextBody dell'oggetto TextBox.

```csharp
public EquationNode GetEquationParagraph()
```

### Valore di ritorno

Se esiste un paragrafo matematico, restituisce il primo, altrimenti restituisce null.

### Esempi

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

### Vedi anche

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


