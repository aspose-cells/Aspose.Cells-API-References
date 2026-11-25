---
title: "Revision.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Revision. Restituisce il numero di questa revisione"
type: docs
url: /it/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Ottiene il numero di questa revisione.

```csharp
public int Id { get; }
```

### Osservazioni

Zero indica che questa revisione non contiene ID.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Apporta una modifica per potenzialmente creare una revisione
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Ottieni la raccolta dei log di revisione
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Ottieni le revisioni dal primo log
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Accedi alla prima revisione
                        Revision revision = revisions[0];
                        
                        // Visualizza la proprietà Id (sola lettura)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Salva la cartella di lavoro
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

### Vedi anche

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


