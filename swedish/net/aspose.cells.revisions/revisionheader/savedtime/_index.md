---
title: "RevisionHeader.SavedTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionHeader‑egenskap. Hämtar och sätter datum och tid då detta revisionsset sparades"
type: docs
url: /sv/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Hämtar och anger datum och tid när detta revisionsset sparades.

```csharp
public DateTime SavedTime { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en revisionshuvudinstans
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Ange egenskapen SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // Hämta och visa värdet SavedTime
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Ändra egenskapen SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Spara arbetsboken för att demonstrera att egenskapen används
                workbook.Save("SavedTimeDemo.xlsx");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


