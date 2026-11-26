---
title: "DelimiterEquationNode.BeginChar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DelimiterEquationNode. Carácter inicial del delimitador"
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

Carácter inicial del delimitador.

```csharp
public string BeginChar { get; set; }
```

### Observaciones

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una ecuación a la primera hoja de cálculo
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Obtener el nodo raíz de la ecuación
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Agregar un nodo delimitador con caracteres inicial/final personalizados
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // Agregar contenido dentro del delimitador
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // Guarda el libro de trabajo
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### Ver también

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


