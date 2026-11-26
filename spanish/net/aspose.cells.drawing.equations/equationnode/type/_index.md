---
title: "EquationNode.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad EquationNode. Representa el tipo del nodo"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/type/
---
## EquationNode.Type property

Representa el tipo del nodo.

```csharp
public override TextNodeType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class EquationNodePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationRoot = shape.GetEquationParagraph();

            // Crear diferentes tipos de nodos de ecuación
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Text";

            // Mostrar la propiedad Type para diferentes nodos
            Console.WriteLine($"Root equation node type: {equationRoot.Type}");
            Console.WriteLine($"Fraction node type: {fractionNode.Type}");
            Console.WriteLine($"Text node type: {textNode.Type}");

            // Crear una estructura de ecuación compleja
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "Numerator";

            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "Denominator";

            // Comprobar los tipos de nodos hijos
            Console.WriteLine($"Numerator node type: {numerator.Type}");
            Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
            Console.WriteLine($"Denominator node type: {denominator.Type}");

            // Demostrar cómo Type afecta el comportamiento del nodo
            if (textNode.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("Text node is a TextRun type - can contain text content");
            }

            if (fractionNode.Type == TextNodeType.Equation)
            {
                Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
            }

            // Guardar el resultado
            workbook.Save("EquationNodePropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


