---
title: "RevisionFormat.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionFormat-egenskap. Hämtar den tillämpade stilen"
type: docs
url: /sv/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Hämtar den tillämpade stilen.

```csharp
public Style Style { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok (revisionsspårning är aktiverad som standard när ändringar görs)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data och formatering för att skapa en revision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Skapa en stil och tillämpa den på cellen
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Kom åt revisionerna via RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Visa de aktuella stil-egenskaperna från revisionen
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Obs: Stil-egenskapen är skrivskyddad i RevisionFormat, så vi kan inte ändra den direkt
                        // För att ändra formatering måste vi ändra cellens stil direkt
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


