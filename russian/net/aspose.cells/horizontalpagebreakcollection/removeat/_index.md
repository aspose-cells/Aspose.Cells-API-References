---
title: "HorizontalPageBreakCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HorizontalPageBreakCollection. Удаляет элемент HPageBreak с указанным именем"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreakcollection/removeat/
---
## HorizontalPageBreakCollection.RemoveAt method

Удаляет элемент HPageBreak с указанным именем.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс элемента, начиная с нуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            worksheet.HorizontalPageBreaks.Add(15);
            
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


