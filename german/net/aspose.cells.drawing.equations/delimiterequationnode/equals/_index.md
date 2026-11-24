---
title: "DelimiterEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DelimiterEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/delimiterequationnode/equals/
---
## DelimiterEquationNode.Equals method

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

    public class DelimiterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei DelimiterEquationNode‑Instanzen zum Vergleich
            // Da DelimiterEquationNode keinen parameterlosen Konstruktor hat,
            // müssen wir sie anders erstellen. Vorausgesetzt, wir können den Standardkonstruktor verwenden
            // der Basisklasse oder einen anderen Weg finden, sie zu erstellen.
            // Zur Demonstration werden wir ObjectCreationHelper (hypothetisch) oder einen ähnlichen Ansatz verwenden
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
                // Rufe die Equals-Methode mit dem Object-Parameter auf
                bool result = node1.Equals((Object)node2);

                // Ergebnis anzeigen
                Console.WriteLine($"Equals method result: {result}");

                // Ändere node2, um sie unterschiedlich zu machen
                node2.BeginChar = "[";
                bool result2 = node1.Equals((Object)node2);
                Console.WriteLine($"Equals method result after modification: {result2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


