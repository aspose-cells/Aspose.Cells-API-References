---
title: "EquationNode.ParentNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad EquationNode. Especifica el nodo padre del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Especifica el nodo padre del nodo actual

```csharp
public EquationNode ParentNode { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodePropertyParentNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear un cuadro de texto con ecuación
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Crear un nodo hijo
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Mostrar los valores de la propiedad ParentNode
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Verificar la relación padre-hijo
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Demostrar la configuración de ParentNode (ya que es de lectura y escritura)
                EquationNode newParent = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
                childNode.ParentNode = newParent;
                Console.WriteLine("After changing parent - Child's new parent: " + (childNode.ParentNode == newParent));

                workbook.Save("ParentNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


