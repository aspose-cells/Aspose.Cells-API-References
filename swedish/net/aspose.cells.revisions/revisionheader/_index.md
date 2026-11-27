---
title: "Klass RevisionHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionHeader class. Representerar en lista över specifika ändringar som har inträffat för den här arbetsboken"
type: docs
url: /sv/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Representerar en lista över specifika ändringar som har inträffat för den här arbetsboken.

```csharp
public class RevisionHeader
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Hämtar och anger datum och tid när detta revisionsset sparades. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Hämtar och anger namnet på användaren som gör revisionen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en instans av RevisionHeader-klassen
                RevisionHeader revisionHeader = new RevisionHeader();

                // Ange nödvändiga egenskaper
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Demonstrera grundläggande funktionalitet
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Spara arbetsboken
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


