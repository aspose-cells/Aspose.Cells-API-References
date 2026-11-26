---
title: "TextBox.GetEquationParagraph"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextBox. Obtenga el párrafo matemático especificado de la propiedad TextBody del objeto TextBox. Aviso 1 Devuelve NULL cuando el índice está fuera de los límites o no se encuentra. 2 También devuelve NULL si la posición de índice especificada no es un párrafo matemático"
type: docs
url: /es/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Obtiene el párrafo matemático especificado de la propiedad TextBody del objeto TextBox. Aviso: (1) Devuelve NULL cuando el índice está fuera de los límites o no se encuentra. (2) También devuelve NULL si la posición del índice especificado no es un párrafo matemático.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de posición del párrafo matemático, comenzando desde 0. |

### Valor de retorno

Devuelve el párrafo matemático especificado por el índice.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Agregar contenido de ecuación al cuadro de texto
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Llamar a GetEquationParagraph con el parámetro de índice (Int32)
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

            // Guarda el libro de trabajo
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Obtiene el primer párrafo matemático de la propiedad TextBody del objeto TextBox.

```csharp
public EquationNode GetEquationParagraph()
```

### Valor de retorno

Si hay un párrafo matemático, devuelve el primero; de lo contrario, devuelve null.

### Ejemplos

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

### Ver también

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


