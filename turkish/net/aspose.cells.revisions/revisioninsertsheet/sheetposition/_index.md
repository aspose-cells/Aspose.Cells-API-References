---
title: "RevisionInsertSheet.SheetPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertSheet özelliği. Yeni sayfanın sayfa sekme çubuğundaki sıfır tabanlı konumunu alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertsheet/sheetposition/
---
## RevisionInsertSheet.SheetPosition property

Yeni sayfanın sayfa sekme çubuğundaki sıfır tabanlı konumunu alır.

```csharp
public int SheetPosition { get; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


