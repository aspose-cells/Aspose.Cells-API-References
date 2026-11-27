---
title: "RevisionFormat.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionFormat egenskap. Hämtar typen av revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Hämtar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok i delat läge för att aktivera revisionsspårning
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data och tillämpa formatering för att skapa en revision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Tillämpa en stil för att skapa en formatrevision
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Åtkomst till revisionsloggarna
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Visa värdet för Type-egenskapen
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Visa ytterligare information om revisionen
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Spara arbetsboken
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

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


