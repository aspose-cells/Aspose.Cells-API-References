---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NaryEquationNode. un operador n-ario, p.ej."
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

un operador n-ario, p.\u202fej. "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accede a la ecuación y agrega un nodo de operador n-ario
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Convierte a NaryEquationNode para acceder a NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Muestra el NaryOperatorType actual (valor predeterminado)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Establece el operador de suma (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Agrega la base (operando) y los límites para demostrar el operador
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Configura el operador para que crezca con su contenido
            naryEquationNode.NaryGrow = true;

            // Cambia al operador de producto (∏) y muestra la diferencia
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Guarda el libro de trabajo
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


