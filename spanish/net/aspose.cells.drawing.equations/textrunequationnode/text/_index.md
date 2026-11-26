---
title: "TextRunEquationNode.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TextRunEquationNode propiedad. Establezca el contenido del nodo de texto. Normalmente un objeto nodo por carácter"
type: docs
url: /es/net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Establecer el contenido del nodo de texto (Normalmente un objeto nodo por carácter).

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextRunEquationNodePropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtenga el nodo raíz de la ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Cree una ecuación fraccionaria
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Agregue el numerador con el texto "X"
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Agregue el denominador con el texto "Y"
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Guarda el libro de trabajo
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            // Verifique el archivo guardado cargándolo nuevamente
            Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Acceda a las propiedades de texto para demostrar la funcionalidad
            TextRunEquationNode loadedNumeratorText = (TextRunEquationNode)((FractionEquationNode)loadedTextBox
                .GetEquationParagraph()
                .GetChild(0)
                .GetChild(0))
                .GetChild(0)
                .GetChild(0);

            Console.WriteLine("Numerator text: " + loadedNumeratorText.Text);
        }
    }
}
```

### Ver también

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


