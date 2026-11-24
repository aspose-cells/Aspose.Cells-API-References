---
title: "RadicalEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadicalEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

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

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie zwei RadicalEquationNode-Instanzen
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // Setzen Sie unterschiedliche Eigenschaften, um den Gleichheitsvergleich zu demonstrieren
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // Vergleichen Sie die Knoten mit der Equals-Methode
                bool areEqual = node1.Equals(node2);

                // Anzeige des Vergleichsergebnisses
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // Vergleichen Sie mit demselben Objekt
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // Vergleiche mit null
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
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

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


