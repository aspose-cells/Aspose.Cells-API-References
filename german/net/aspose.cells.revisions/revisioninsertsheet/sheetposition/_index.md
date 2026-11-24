---
title: "RevisionInsertSheet.SheetPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertSheet‑Eigenschaft. Gibt die nullbasierte Position des neuen Blatts in der Registerkartenleiste zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertsheet/sheetposition/
---
## RevisionInsertSheet.SheetPosition property

Liest die nullbasierte Position des neuen Blatts in der Blattregisterleiste.

```csharp
public int SheetPosition { get; }
```

### Beispiele

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

### Siehe auch

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


