---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DelimiterEquationNode. Especifica la forma de los delimitadores en el objeto delimitador"
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Especifica la forma de los delimitadores en el objeto delimitador.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyDelimiterShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtener el nodo de ecuación
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear nodo delimitador con forma personalizada
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // Agregar contenido dentro del delimitador
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // Guarda el libro de trabajo
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### Ver también

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


