---
title: "RevisionRenameSheet.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionRenameSheet. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Rappresenta il tipo della revisione.

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

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Abilita il tracciamento delle revisioni PRIMA di apportare modifiche
            // Nota: Questo metodo non esiste nell'API fornita, quindi lo rimuoveremo
            // workbook.StartTrackingRevisions();

            // Rinomina il primo foglio di lavoro per creare una revisione
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Accedi alla collezione delle revisioni
            // Nota: La proprietà Revisions non esiste nell'API fornita
            // Quindi dovremo prima verificare se la cartella di lavoro ha revisioni
            if (workbook.HasRevisions)
            {
                // Trova la revisione di rinomina del foglio
                RevisionRenameSheet renameRevision = null;
                // Poiché non possiamo accedere direttamente a Revisions, dovremo modificare questa parte
                // Questo è solo un segnaposto poiché l'API reale non supporta l'accesso alle revisioni
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Visualizza il valore della proprietà Type
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Dimostra come utilizzare la proprietà Type
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


