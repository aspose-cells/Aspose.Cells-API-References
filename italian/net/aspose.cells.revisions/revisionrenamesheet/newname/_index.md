---
title: "RevisionRenameSheet.NewName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionRenameSheet. Ottiene il nuovo nome del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

Ottiene il nuovo nome del foglio di lavoro.

```csharp
public string NewName { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyNewNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e rinominalo per generare una revisione
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

            // Salva in un flusso di memoria per generare revisioni
            System.IO.MemoryStream ms = new System.IO.MemoryStream();
            workbook.Save(ms, SaveFormat.Xlsx);

            // Riapri la cartella di lavoro per accedere ai registri delle revisioni
            workbook = new Workbook(ms);
            
            // Verifica i registri delle revisioni per l'operazione di rinomina
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // Dimostra l'uso della proprietà NewName
                        if (renameSheet.NewName == newName)
                        {
                            Console.WriteLine("NewName property verification successful");
                        }
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


