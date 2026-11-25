---
title: "RevisionRenameSheet.OldName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionRenameSheet. Ottiene il vecchio nome del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisionrenamesheet/oldname/
---
## RevisionRenameSheet.OldName property

Ottiene il vecchio nome del foglio di lavoro.

```csharp
public string OldName { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyOldNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e rinominalo per generare una revisione
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            sheet.Name = "RenamedSheet";

            // Accedi ai registri delle revisioni
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from: {0} to: {1}", rsnm.OldName, rsnm.NewName);
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


