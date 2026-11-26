---
title: "DelimiterEquationNode.NaryGrow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DelimiterEquationNode. Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula"
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/narygrow/
---
## DelimiterEquationNode.NaryGrow property

Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula.

```csharp
public bool NaryGrow { get; set; }
```

### Observaciones

Esta propiedad especifica la característica de crecimiento del delimitador a nivel de documento. Cuando está desactivada, el delimitador no crecerá para coincidir con el tamaño de la altura de su componente. Cuando está habilitada, el delimitador crece verticalmente para coincidir con la altura de su componente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            var paragraph = textBox.GetEquationParagraph();
            var mathNode = paragraph.GetChild(0);
            
            // Crear nodo delimitador con la propiedad NaryGrow
            var delimiterNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Delimiter) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            delimiterNode.DelimiterShape = Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType.Match;
            delimiterNode.NaryGrow = false; // Demonstrating NaryGrow property
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            delimiterNode.SeparatorChar = ",";

            // Agregar elementos base
            var baseNode1 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode1 = baseNode1.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode1.Text = "x";

            var baseNode2 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode2 = baseNode2.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode2.Text = "y";

            // Guardar y verificar
            string outputFile = "DelimiterEquationNode_NaryGrow_Demo.xlsx";
            workbook.Save(outputFile);

            // Verifique el archivo guardado
            Workbook verifyWorkbook = new Workbook(outputFile);
            var verifyTextBox = verifyWorkbook.Worksheets[0].Shapes[0] as Aspose.Cells.Drawing.TextBox;
            var verifyNode = verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            
            Console.WriteLine("NaryGrow value: " + verifyNode.NaryGrow); // Should output "False"
        }
    }
}
```

### Ver también

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


