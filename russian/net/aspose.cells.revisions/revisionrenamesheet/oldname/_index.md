---
title: "RevisionRenameSheet.OldName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionRenameSheet. Возвращает старое имя листа"
type: docs
url: /ru/net/aspose.cells.revisions/revisionrenamesheet/oldname/
---
## RevisionRenameSheet.OldName property

Получает старое имя листа.

```csharp
public string OldName { get; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и переименуйте его, чтобы вызвать ревизию
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            sheet.Name = "RenamedSheet";

            // Получите доступ к журналам ревизий
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

### См. также

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


