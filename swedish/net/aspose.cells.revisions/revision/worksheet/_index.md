---
title: "Revision.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Revision egenskap. Hämtar arbetsbladet"
type: docs
url: /sv/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Hämtar kalkylbladet.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in kalkylblads egenskaper
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Lägg till data för att demonstrera revisioner
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Skydda arbetsbladet för att möjliggöra spårning av ändringar
            worksheet.Protect(ProtectionType.All);
            
            // Gör en ändring som kommer att spåras som revision
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Spara arbetsboken för att spåra revisioner
            workbook.Save("RevisionDemo.xlsx");
            
            // Läs in arbetsboken med revisioner
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Kom åt revisionsloggar
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Demonstrera åtkomst till Worksheet-egenskapen från revision
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


