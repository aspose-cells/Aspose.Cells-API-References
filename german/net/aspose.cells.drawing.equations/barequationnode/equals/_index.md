---
title: "BarEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BarEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist."
type: docs
url: /de/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie zwei BarEquationNode-Instanzen zum Vergleich
            // Hinweis: Die tatsächliche Erstellung von BarEquationNode hängt von den Fabrikmethoden der API ab.
            // Zur Demonstration gehen wir davon aus, dass dies korrekt initialisierte Instanzen sind.
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Vergleiche node1 mit node2 (sollte gleich sein)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Vergleiche node1 mit node3 (sollte nicht gleich sein)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Vergleiche node1 mit null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Vergleiche node1 mit einem anderen Objekttyp
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Hilfsmethode, um das Abrufen eines BarEquationNode zu demonstrieren
        // In der realen Anwendung würden Sie die passende API-Methode verwenden, um diese zu erstellen
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Dies ist nur ein Platzhalter – die tatsächliche Implementierung würde von der API abhängen
            // Zum Beispiel könnte es über ein übergeordnetes Objekt oder eine Fabrikmethode erstellt werden
            return null; // Replace with actual creation code
        }
    }
}
```

### Siehe auch

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


