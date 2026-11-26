---
title: "Enum EquationCharacterPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationCharacterPositionType enum. Especifica la posición de un subobjeto particular dentro de su padre"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

Especifica la posición de un subobjeto particular dentro de su padre

```csharp
public enum EquationCharacterPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Top | `0` | En la parte superior del objeto padre |
| Bottom | `1` | En la parte inferior del objeto padre |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCharacterPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtener el nodo de ecuación y agregar barra con posición superior
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            barNode.BarPosition = EquationCharacterPositionType.Top;
            
            // Agregar texto base
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";
            
            // Guardar y verificar
            string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
            workbook.Save(outputFile);
            
            // Recargar y verificar
            Workbook loadedWorkbook = new Workbook(outputFile);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
            Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


