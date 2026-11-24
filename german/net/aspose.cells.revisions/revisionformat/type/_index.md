---
title: "RevisionFormat.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionFormat-Eigenschaft. Gibt den Typ der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Liest den Typ der Revision.

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

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe im Freigabemodus, um die Revisionsverfolgung zu aktivieren
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu und wende Formatierung an, um eine Revision zu erzeugen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Wende einen Stil an, um eine Formatierungsrevision zu erstellen
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Greife auf die Revisionsprotokolle zu
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Den Wert der Type-Eigenschaft anzeigen
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Zusätzliche Informationen zur Revision anzeigen
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


