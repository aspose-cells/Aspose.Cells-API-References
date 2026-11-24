---
title: "RevisionQueryTable.CellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionQueryTable‑Eigenschaft. Gibt den Speicherort der betroffenen Abfrage‑Tabelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Ermittelt den Speicherort der betroffenen Abfrage‑Tabelle.

```csharp
public CellArea CellArea { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // In einem echten Szenario würden Sie Revisionen aus der Arbeitsmappe erhalten
                // Zur Demonstration erstellen wir ein konzeptionelles Beispiel
                // Hinweis: RevisionQueryTable‑Instanzen werden typischerweise aus Arbeitsmappen‑Revisionen erhalten
                RevisionQueryTable revisionQueryTable = null;

                // Überprüfen Sie, ob wir eine RevisionQueryTable haben
                if (revisionQueryTable != null)
                {
                    // Zeigen Sie den Wert der CellArea‑Eigenschaft an (schreibgeschützt)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Zeige weitere Eigenschaften für den Kontext an
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("CellAreaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


