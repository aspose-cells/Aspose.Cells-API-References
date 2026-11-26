---
title: "EquationNode.InsertAfter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Inserta el nodo especificado después del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Inserta el nodo especificado después del nodo actual.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | EquationNodeType | Tipos de nodos de ecuación |

### Valor de retorno

Si el tipo especificado existe, se devuelve el nodo correspondiente, y si el tipo no existe, se devuelve un nodo de tipo desconocido.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ecuación en la celda A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Agregar nodo de texto inicial
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Insertar un nuevo nodo de texto después del existente
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Mostrar la estructura de la ecuación
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Guardar la ecuación en una celda para inspección visual
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


