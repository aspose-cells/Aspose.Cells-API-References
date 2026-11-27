---
title: "Klass RevisionFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionFormat-klass. Representerar en revisionspost med information om en formateringsändring"
type: docs
url: /sv/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Representerar en revisionspost med information om en formateringsändring.

```csharp
public class RevisionFormat : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | Det område som denna formatering tillämpades på. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Hämtar den tillämpade stilen. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

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
            // Skapa en ny arbetsbok i delat läge för att aktivera revisionsspårning
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till data och tillämpa formatering för att skapa en revision
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Tillämpa en stil för att skapa en formatrevision
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Åtkomst till revisionsloggarna
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Visa revisionsegenskaperna
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Visa stilinformation
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Spara arbetsboken
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

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


