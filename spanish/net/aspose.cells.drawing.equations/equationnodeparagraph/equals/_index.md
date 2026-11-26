---
title: "EquationNodeParagraph.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNodeParagraph. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dos instancias de EquationNodeParagraph para comparar
            // Usando el método CreateNode para instanciar correctamente los nodos
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Establece diferentes tipos de justificación para que sean desiguales
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Llama al método Equals con paragraph2 como parámetro
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Mostrar el resultado de la comparación
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // Crea otro párrafo con la misma justificación que paragraph1
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Llama a Equals nuevamente con paragraph3
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // También demuestra la comparación con null
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo (aunque no se realizaron cambios visibles en la hoja de cálculo)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


