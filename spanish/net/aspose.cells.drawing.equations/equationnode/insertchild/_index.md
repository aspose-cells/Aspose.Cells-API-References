---
title: "EquationNode.InsertChild"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | valor de índice |
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

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Agregar nodo de texto inicial a la ecuación
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Insertar un nuevo nodo de fracción en el índice 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Guarda el libro de trabajo
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


