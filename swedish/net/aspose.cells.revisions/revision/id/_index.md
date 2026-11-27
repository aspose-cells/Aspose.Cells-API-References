---
title: "Revision.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Revision egenskap. Hämtar numret för denna revision"
type: docs
url: /sv/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Hämtar numret för denna revision.

```csharp
public int Id { get; }
```

### Anmärkningar

Noll betyder att denna revision inte innehåller ett id.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gör en ändring för att eventuellt skapa en revision
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Hämta samlingen av revisionsloggar
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Hämta revisioner från den första loggen
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Kom åt den första revisionen
                        Revision revision = revisions[0];
                        
                        // Visa Id-egenskapen (skrivskyddad)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Spara arbetsboken
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
                }
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

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


