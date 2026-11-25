---
title: "RevisionCustomView.Guid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCustomView. Ottiene l'identificatore univoco globale della vista personalizzata"
type: docs
url: /it/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Ottiene l'identificatore univoco globale della vista personalizzata.

```csharp
public Guid Guid { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // Apri una cartella di lavoro esistente che contiene revisioni di vista personalizzata
            Workbook workbook = new Workbook("example.xlsx");
            
            // Elabora i registri di revisione
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


