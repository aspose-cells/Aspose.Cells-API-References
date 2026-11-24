---
title: "BoxEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BoxEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist."
type: docs
url: /de/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie zwei BoxEquationNode-Objekte zum Vergleich
            // Da BoxEquationNode keinen parameterlosen Konstruktor hat,
            // müssen wir sie anders erstellen. Angenommen, wir können sie irgendwoher erhalten,
            // oder sie mit einigen Standardparametern erstellen.
            // Für Demonstrationszwecke deklarieren wir sie einfach und setzen sie auf null (obwohl im echten Code eine korrekte Initialisierung erforderlich wäre)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Rufen Sie die Equals-Methode mit den spezifischen Parametertypen (Object) auf
                    bool areEqual = node1.Equals(objToCompare);

                    // Ergebnis anzeigen
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Füge das Ergebnis dem Arbeitsblatt hinzu
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Ergebnis speichern
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


