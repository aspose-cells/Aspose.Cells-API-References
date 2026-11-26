---
title: "DelimiterEquationNode.EndChar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DelimiterEquationNode. Carácter final del delimitador"
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

Carácter final del delimitador.

```csharp
public string EndChar { get; set; }
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
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtener el nodo de ecuación
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear un nodo delimitador con carácter final personalizado
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // Agregar contenido dentro del delimitador
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // Guardar y verificar
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Verifique el archivo guardado
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### Ver también

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


