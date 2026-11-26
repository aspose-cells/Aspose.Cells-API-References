---
title: "Enum EquationHorizontalJustificationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. Esto especifica la justificación horizontal predeterminada de las ecuaciones en el documento"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

Esto especifica la justificación horizontal predeterminada de las ecuaciones en el documento.

```csharp
public enum EquationHorizontalJustificationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Center | `0` | Centrado |
| CenterGroup | `1` | Centrado como Grupo |
| Left | `2` | Alineado a la izquierda |
| Right | `3` | Alineado a la derecha |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma de ecuación a la hoja de cálculo
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Obtener el párrafo de la ecuación
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // Demostrar diferentes tipos de justificación horizontal
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // Guarda el libro de trabajo
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


