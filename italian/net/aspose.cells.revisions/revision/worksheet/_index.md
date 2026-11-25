---
title: "Revision.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Revision. Restituisce il foglio di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Ottiene il foglio di lavoro.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le proprietà del worksheet
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Aggiungi alcuni dati per dimostrare le revisioni
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Proteggi il foglio di lavoro per abilitare il tracciamento delle modifiche
            worksheet.Protect(ProtectionType.All);
            
            // Apporta una modifica che verrà tracciata come revisione
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Salva la cartella di lavoro per tracciare le revisioni
            workbook.Save("RevisionDemo.xlsx");
            
            // Carica la cartella di lavoro con le revisioni
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Accedi ai log delle revisioni
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Dimostra l'accesso alla proprietà Worksheet dalla revisione
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

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


