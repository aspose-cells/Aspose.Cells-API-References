---
title: "RevisionCustomView.Guid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCustomView. Получает глобальный уникальный идентификатор пользовательского представления"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Получает глобальный уникальный идентификатор пользовательского представления.

```csharp
public Guid Guid { get; }
```

### Примеры

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
            // Открыть существующую книгу, содержащую ревизии пользовательского представления
            Workbook workbook = new Workbook("example.xlsx");
            
            // Обрабатывать журналы ревизий
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

### См. также

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


