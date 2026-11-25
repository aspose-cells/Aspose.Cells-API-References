---
title: "EquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Determina se il nodo di equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/equals/
---
## EquationNode.Equals method

Determina se il nodo dell'equazione corrente è uguale al nodo specificato

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | Il nodo specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due nodi di equazione per il confronto
            EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

            try
            {
                // Chiama il metodo Equals con parametro Object
                bool areEqual = node1.Equals((object)node2);

                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Modifica node2 per renderli diversi
                node2.AddChild(EquationNodeType.Base);

                areEqual = node1.Equals((object)node2);
                Console.WriteLine($"After modification, are they equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("EquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


