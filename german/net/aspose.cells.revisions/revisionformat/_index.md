---
title: "Klasse RevisionFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionFormat Klasse. Stellt einen Revisionsdatensatz mit Informationen zu einer Formatierungsänderung dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Stellt einen Revisionsdatensatz mit Informationen über eine Formatierungsänderung dar.

```csharp
public class RevisionFormat : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | Der Bereich, auf den diese Formatierung angewendet wurde. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Liest den angewendeten Stil. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Liest den Typ der Revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe im Freigabemodus, um die Revisionsverfolgung zu aktivieren
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge einige Daten hinzu und wende Formatierung an, um eine Revision zu erzeugen
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Wende einen Stil an, um eine Formatierungsrevision zu erstellen
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Greife auf die Revisionsprotokolle zu
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Zeige die Revisions-Eigenschaften an
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Zeige Stilinformationen an
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


