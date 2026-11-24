---
title: "Revision.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Revision-Eigenschaft. Gibt die Nummer dieser Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Gibt die Nummer dieser Revision zurück.

```csharp
public int Id { get; }
```

### Hinweise

Null bedeutet, dass diese Revision keine ID enthält.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nehmen Sie eine Änderung vor, um möglicherweise eine Revision zu erstellen
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Abrufen der Revisionsprotokollsammlung
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Abrufen von Revisionen aus dem ersten Protokoll
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Zugriff auf die erste Revision
                        Revision revision = revisions[0];
                        
                        // Anzeige der Id-Eigenschaft (schreibgeschützt)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


