---
title: "RevisionHeader.SavedTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionHeader. Ottiene e imposta la data e l'ora in cui questo insieme di revisioni è stato salvato"
type: docs
url: /it/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Ottiene e imposta la data e l'ora in cui questo insieme di revisioni è stato salvato.

```csharp
public DateTime SavedTime { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un'istanza di revision header
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Imposta la proprietà SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // Ottieni e visualizza il valore SavedTime
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Modifica la proprietà SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Salva la cartella di lavoro per dimostrare che la proprietà è in uso
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

### Vedi anche

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


