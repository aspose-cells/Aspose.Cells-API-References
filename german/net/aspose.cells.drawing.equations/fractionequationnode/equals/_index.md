---
title: "FractionEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FractionEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Da FractionEquationNode keinen parameterlosen Konstruktor hat,
                // werden wir Equals mit Objekten demonstrieren, die vermutlich aus anderen Teilen der API stammen
                // Zu Demonstrationszwecken gehen wir davon aus, dass wir zwei zu vergleichende Instanzen haben
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Vergleichen Sie die Objekte mit Equals
                bool areEqual = node1.Equals(node2);

                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Vergleiche mit null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Mit sich selbst vergleichen
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Hilfsmethode, um das Abrufen von FractionEquationNode-Instanzen zu simulieren
        // (Im realen Einsatz würden diese von der API kommen)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Dies ist nur ein Platzhalter – in Wirklichkeit würden Sie diese von der API erhalten
            // Zum Beispiel: worksheet.Equations.AddFractionEquationNode() oder ähnlich
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Siehe auch

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


