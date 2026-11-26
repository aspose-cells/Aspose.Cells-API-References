---
title: "RevisionInsertSheet.SheetPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertSheet. Возвращает нулевую позицию нового листа в панели вкладок листов"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertsheet/sheetposition/
---
## RevisionInsertSheet.SheetPosition property

Получает нулевую позицию нового листа на панели вкладок листов.

```csharp
public int SheetPosition { get; }
```

### Примеры

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

### См. также

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


