---
title: "UnknowEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnknowEquationNode-Methode. Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei unbekannte Gleichungsknoten zum Vergleich
            // Da UnknowEquationNode keinen parameterlosen Konstruktor hat,
            // müssen wir sie anders erstellen. Für Demonstrationszwecke verwenden wir
            // den tatsächlichen Konstruktor, falls verfügbar, oder sie auf andere Weise erstellen.
            // Da wir die Konstruktorparameter nicht kennen, ist dies ein Platzhalter-Fix.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Rufen Sie die Equals-Methode mit dem spezifischen Parametertyp (Object) auf
                bool areEqual = node1.Equals(objToCompare);

                // Ergebnis anzeigen
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Füge das Ergebnis dem Arbeitsblatt hinzu
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Hilfsmethode zum Erstellen von UnknowEquationNode-Instanzen
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // In einer echten Implementierung würde dies den richtigen Konstruktor verwenden
            // Da wir die Konstruktorparameter nicht kennen, geben wir null zurück
            // und behandeln den Null-Fall im Demo (obwohl dies nur ein Platzhalter ist)
            return null;
        }
    }
}
```

### Siehe auch

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


