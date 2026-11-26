---
title: "Enum EquationLimitLocationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Especifica la ubicación del límite en un operador"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Especifica la ubicación del límite en un operador.

```csharp
public enum EquationLimitLocationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| UndOvr | `0` | Especifica que el límite está centrado arriba o abajo del operador. |
| SubSup | `1` | Especifica que el límite está en el lado derecho del operador. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma de ecuación a la hoja de cálculo
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Obtener el párrafo de la ecuación y su primer hijo
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Crear un nodo de ecuación Nary
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Establecer la ubicación del límite a SubSup (lado derecho del operador)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Agregar contenido a la ecuación
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Cambiar a UndOvr (centrado arriba/abajo del operador)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Guarda el libro de trabajo
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


