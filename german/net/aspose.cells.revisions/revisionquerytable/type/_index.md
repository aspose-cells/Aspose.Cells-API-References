---
title: "RevisionQueryTable.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionQueryTable-Eigenschaft. Repräsentiert den Typ der Revision"
type: docs
url: /de/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Stellt den Typ der Revision dar.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyTypeDemo
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

                // Erstellen Sie eine Mock-RevisionQueryTable (dies ist konzeptionell – in der Realität würden Sie sie aus Revisionen erhalten)
                // Da wir RevisionQueryTable nicht direkt instanziieren können, zeigen wir das Muster
                RevisionQueryTable revisionQueryTable = null;

                // Überprüfen Sie, ob wir eine RevisionQueryTable haben
                if (revisionQueryTable != null)
                {
                    // Zeigen Sie den Wert der Type‑Eigenschaft an (schreibgeschützt)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Zeigen Sie den Enum‑Wert als Ganzzahl zum Nachschlagen an
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Zeige weitere Eigenschaften für den Kontext an
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Speichere die Arbeitsmappe
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


