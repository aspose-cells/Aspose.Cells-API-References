---
title: "RevisionInsertSheet.SheetPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertSheet. Restituisce la posizione basata su zero del nuovo foglio nella barra delle schede"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertsheet/sheetposition/
---
## RevisionInsertSheet.SheetPosition property

Ottiene la posizione basata su zero del nuovo foglio nella barra delle schede dei fogli.

```csharp
public int SheetPosition { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionInsertSheetPropertySheetPositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet insertedSheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            insertedSheet.Name = "NewSheet";

            workbook.Save("revisions_sample.xlsx");

            Workbook reopenedWorkbook = new Workbook("revisions_sample.xlsx");
            foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertSheet)
                    {
                        RevisionInsertSheet ris = (RevisionInsertSheet)revision;
                        Console.WriteLine($"Sheet Name: {ris.Name}, Position: {ris.SheetPosition}");
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


