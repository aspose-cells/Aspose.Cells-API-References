---
title: "DelimiterEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DelimiterEquationNode. Determina se il nodo equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/delimiterequationnode/equals/
---
## DelimiterEquationNode.Equals method

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

    public class DelimiterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due istanze di DelimiterEquationNode per il confronto
            // Poiché DelimiterEquationNode non ha un costruttore senza parametri,
            // dovremo crearli in modo diverso. Supponendo di poter utilizzare il costruttore predefinito
            // della classe base o trovare un altro modo per crearli.
            // Per dimostrazione, utilizzeremo ObjectCreationHelper (ipotetico) o un approccio simile
            DelimiterEquationNode node1 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node1.BeginChar = "(";
            node1.EndChar = ")";
            node1.SeparatorChar = ",";
            node1.DelimiterShape = EquationDelimiterShapeType.Centered;

            DelimiterEquationNode node2 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node2.BeginChar = "(";
            node2.EndChar = ")";
            node2.SeparatorChar = ",";
            node2.DelimiterShape = EquationDelimiterShapeType.Centered;

            try
            {
                // Chiama il metodo Equals con parametro Object
                bool result = node1.Equals((Object)node2);

                // Visualizza il risultato
                Console.WriteLine($"Equals method result: {result}");

                // Modifica node2 per renderli diversi
                node2.BeginChar = "[";
                bool result2 = node1.Equals((Object)node2);
                Console.WriteLine($"Equals method result after modification: {result2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


