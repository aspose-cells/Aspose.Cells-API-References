---
title: "RevisionLog.MetadataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionLog-egenskap. Hämtar tabellen som innehåller metadata om en lista med specifika ändringar som har skett för denna arbetsbok"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Hämtar tabellen som innehåller metadata om en lista med specifika ändringar som har inträffat för den här arbetsboken.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gör några ändringar för att skapa revisionshistorik
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Modifiera cellen för att skapa en revision
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Öppna den modifierade arbetsboken igen för att komma åt revisionsloggar
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Kom åt revisionsloggar
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### Se även

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


