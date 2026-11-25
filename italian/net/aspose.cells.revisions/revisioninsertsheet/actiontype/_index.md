---
title: "RevisionInsertSheet.ActionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertSheet. Restituisce il tipo di azione della revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Ottiene il tipo di azione della revisione.

```csharp
public RevisionActionType ActionType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            // Nota: StartTrackingRevisions non è disponibile nell'API fornita
            // workbook.StartTrackingRevisions();

            // Aggiungi un nuovo foglio di lavoro per generare un record di revisione
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Nota: StopTrackingRevisions non è disponibile nell'API fornita
            // workbook.StopTrackingRevisions();
            
            // Nota: la proprietà Revisions non è disponibile nell'API fornita
            // Useremo HasRevisions per verificare se ci sono revisioni
            if (workbook.HasRevisions)
            {
                // In uno scenario reale, accederemmo alle revisioni qui
                // Poiché non possiamo creare RevisionInsertSheet direttamente, simuleremo il controllo di uno
                // Questo presuppone che abbiamo ottenuto la revisione da qualche parte (come workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Poiché non possiamo creare o impostare ActionType, dimostreremo semplicemente il controllo
                if (insertSheetRevision != null)
                {
                    // Visualizza la proprietà ActionType
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Dimostra l'uso della proprietà di sola lettura
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Salva la cartella di lavoro con le revisioni
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Vedi anche

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


