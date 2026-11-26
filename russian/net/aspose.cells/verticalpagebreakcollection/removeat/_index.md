---
title: "VerticalPageBreakCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VerticalPageBreakCollection. Удаляет элемент VPageBreak с указанным именем"
type: docs
url: /ru/net/aspose.cells/verticalpagebreakcollection/removeat/
---
## VerticalPageBreakCollection.RemoveAt method

Удаляет элемент VPageBreak с указанным именем.

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
    public class VerticalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            verticalPageBreaks.RemoveAt(1);

            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
            }

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


