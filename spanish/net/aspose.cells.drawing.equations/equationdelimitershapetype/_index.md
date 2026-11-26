---
title: "Enumeración EquationDelimiterShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType. Esto especifica la forma de los delimitadores en el objeto delimitador"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Esto especifica la forma de los delimitadores en el objeto delimitador.

```csharp
public enum EquationDelimiterShapeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Centered | `0` | El divisor está centrado alrededor de toda la altura de su contenido. |
| Match | `1` | El divisor se ajusta para coincidir exactamente con la altura de sus contenidos. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Obtener nodo de ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crear nodo delimitador con tipo de forma Match
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Agregar contenido dentro del delimitador
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Guarda el libro de trabajo
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


