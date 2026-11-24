---
title: "BorderBoxEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderBoxEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie zwei BorderBoxEquationNode-Instanzen zum Vergleich
                // Da BorderBoxEquationNode keinen parameterlosen Konstruktor hat,
                // verwenden wir den Basisklassenkonstruktor (unter der Annahme, dass EquationNode einen hat)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Vergleichen Sie die Knoten mit der Equals-Methode
                bool areEqual = node1.Equals((object)node2);
                
                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Vergleichen Sie mit einem anderen Objekttyp
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


