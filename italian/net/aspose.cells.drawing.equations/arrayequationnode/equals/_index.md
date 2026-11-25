---
title: "ArrayEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ArrayEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/arrayequationnode/equals/
---
## ArrayEquationNode.Equals method

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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class ArrayEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due nodi di equazione array
            ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
            ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // Aggiungi nodi figlio per renderli diversi
            EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
            // Usa ToLaTeX() o ToMathML() invece della proprietà Value
            arrayEquation1.AddChild(child1);

            EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
            arrayEquation2.AddChild(child2);

            try
            {
                // Chiama il metodo Equals con oggetti diversi
                bool result1 = arrayEquation1.Equals(arrayEquation2);
                Console.WriteLine($"Comparing different array equations: {result1}");

                // Chiama Equals con lo stesso oggetto
                bool result2 = arrayEquation1.Equals(arrayEquation1);
                Console.WriteLine($"Comparing same array equation: {result2}");

                // Chiama Equals con null
                bool result4 = arrayEquation1.Equals(null);
                Console.WriteLine($"Comparing with null: {result4}");
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


