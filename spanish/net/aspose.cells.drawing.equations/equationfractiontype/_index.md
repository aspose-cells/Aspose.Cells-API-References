---
title: "Enumeración EquationFractionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationFractionType enumeración. Esto especifica el estilo de visualización de la barra de fracción"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Esto especifica el estilo de visualización de la barra de fracción.

```csharp
public enum EquationFractionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Bar | `0` | Esto especifica que el numerador está arriba y el denominador abajo, separados por una barra en el medio. |
| NoBar | `1` | Esto especifica que el numerador está arriba y el denominador abajo, sin estar separados por una barra en el medio. |
| Linear | `2` | Esto especifica que el numerador está a la izquierda y el denominador a la derecha, separados por un '/' entre ambos. |
| Skewed | `3` | Esto especifica que el numerador está en la esquina superior izquierda y el denominador en la esquina inferior derecha, separados por un "/". |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenga el nodo matemático y agregue la fracción
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Agregar numerador
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Agregar denominador
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Guardar y verificar
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


