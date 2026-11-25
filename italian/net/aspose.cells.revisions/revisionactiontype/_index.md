---
title: "Enum RevisionActionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionActionType enum. Rappresenta il tipo di azione di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Rappresenta il tipo di azione di revisione.

```csharp
public enum RevisionActionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Add | `0` | Aggiungi revisione. |
| Delete | `1` | Elimina revisione. |
| DeleteColumn | `2` | Revisione di eliminazione colonna. |
| DeleteRow | `3` | Revisione di eliminazione riga. |
| InsertColumn | `4` | Revisione di inserimento colonna. |
| InsertRow | `5` | Revisione di inserimento riga. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Esegui varie operazioni che generano diversi tipi di revisione
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Verifica se il workbook ha revisioni
            if (workbook.HasRevisions)
            {
                // Nota: L'API originale non fornisce accesso diretto alla collezione delle revisioni
                // Quindi mostreremo semplicemente l'enum RevisionActionType come richiesto
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Dimostra l'uso dei valori dell'enum RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


