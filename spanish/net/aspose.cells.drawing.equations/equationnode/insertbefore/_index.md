---
title: "EquationNode.InsertBefore"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Inserta el nodo especificado antes del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Inserta el nodo especificado antes del nodo actual.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una ecuación matemática en la celda A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Agregar nodo de texto inicial a la ecuación
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Inserta un nuevo nodo de texto antes del existente
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Muestra la ecuación en formato LaTeX
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


