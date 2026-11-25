---
title: "RevisionMergeConflict.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionMergeConflict. Ottiene il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

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

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita il tracciamento delle modifiche
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Apporta modifiche per creare uno scenario di conflitto di unione
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Simula un conflitto di unione aprendo il file e apportando modifiche conflittuali
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Unisci le modifiche conflittuali
            workbook.Combine(otherUserWorkbook);

            // Verifica se ci sono revisioni
            if (workbook.HasRevisions)
            {
                // Trova la revisione del conflitto di unione
                RevisionMergeConflict mergeConflictRevision = null;
                // Nota: Nell'implementazione reale, avresti bisogno di un altro modo per accedere alle revisioni
                // poiché la proprietà Revisions non è disponibile nella definizione API fornita

                if (mergeConflictRevision != null)
                {
                    // Visualizza la proprietà Type della revisione del conflitto di unione
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Dimostra come queste informazioni possono essere utilizzate
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


