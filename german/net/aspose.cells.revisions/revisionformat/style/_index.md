---
title: "RevisionFormat.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionFormat-Eigenschaft. Gibt den angewendeten Stil zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Liest den angewendeten Stil.

```csharp
public Style Style { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Erstellen Sie ein neues Arbeitsbuch (die Revisionsverfolgung ist standardmäßig aktiviert, wenn Änderungen vorgenommen werden)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten und Formatierungen hinzu, um eine Revision zu erstellen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Erstelle einen Stil und wende ihn auf die Zelle an
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Greifen Sie über RevisionLogs auf die Revisionen zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Zeigen Sie die aktuellen Stileigenschaften der Revision an
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Hinweis: Die Style-Eigenschaft ist in RevisionFormat schreibgeschützt, daher können wir sie nicht direkt ändern
                        // Um die Formatierung zu ändern, müssten wir den Zellenstil direkt anpassen
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


