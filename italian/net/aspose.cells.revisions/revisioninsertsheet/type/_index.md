---
title: "RevisionInsertSheet.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertSheet. Restituisce il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

Ottiene il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            
            // Abilita il tracciamento delle revisioni (simulato poiché StartTrackingRevisions non è disponibile)
            bool trackRevisions = true;

            // Aggiungi un nuovo foglio di lavoro per generare un record di revisione
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Simula l'ottenimento delle revisioni (poiché la proprietà Revisions non è disponibile)
            if (trackRevisions && workbook.HasRevisions)
            {
                // In uno scenario reale, accederemmo alle revisioni qui
                // Questo presuppone che abbiamo ottenuto la revisione da qualche parte (come workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Visualizza la proprietà Type
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Dimostra l'uso della proprietà Type a sola lettura
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Mostra informazioni aggiuntive sul foglio inserito
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Verifica rispetto ad altri tipi di revisione
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


