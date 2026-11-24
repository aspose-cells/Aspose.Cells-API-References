---
title: "TextRunEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextRunEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zu Demonstrationszwecken verwenden wir null und zeigen lediglich die Vergleichslogik
            // da wir TextRunEquationNode-Instanzen nicht direkt erstellen können
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Dieser Teil bleibt, um zu zeigen, wie Equals aufgerufen werden würde
                // In einem realen Szenario würden diese Knoten ordnungsgemäß initialisiert werden
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Vergleiche node1 mit node2 (gleicher Inhalt)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Vergleiche node1 mit node3 (unterschiedlicher Inhalt)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Vergleiche mit null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Vergleichen mit einem anderen Objekttyp
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Arbeitsmappe speichern (obwohl Equals das Tabellenblatt nicht ändert)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Hilfsmethode entfernt, da wir TextRunEquationNode-Instanzen nicht korrekt erstellen können
    }
}
```

### Siehe auch

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


