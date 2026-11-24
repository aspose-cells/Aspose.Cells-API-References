---
title: "MathematicalEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MathematicalEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist."
type: docs
url: /de/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle zwei MathematicalEquationNode-Instanzen zum Vergleich
                // Da MathematicalEquationNode keinen parameterlosen Konstruktor hat,
                // müssen wir null oder geeignete Parameter übergeben
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Vergleichen Sie die Knoten mit der Equals-Methode
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Vergleichen Sie mit einem anderen Objekttyp
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


