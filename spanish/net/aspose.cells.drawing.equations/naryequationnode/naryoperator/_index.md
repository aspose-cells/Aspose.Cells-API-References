---
title: "NaryEquationNode.NaryOperator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NaryEquationNode. un operador nary, p. ej. Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador nary. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido."
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

un operador n-ario, p.\u202fej. "∑". Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido.

```csharp
public string NaryOperator { get; set; }
```

### Observaciones

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el nodo de ecuación
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear un nodo de operador n-ario
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Establecer propiedades del operador n-ario
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Agregar subíndice (opcional)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Agregar superíndice (opcional)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Agregar expresión base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Guarda el libro de trabajo
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Ver también

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


