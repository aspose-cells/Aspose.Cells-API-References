---
title: "Range.UnMerge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Разъединяет объединённые ячейки этого диапазона"
type: docs
url: /ru/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Разъединяет объединённые ячейки этого диапазона.

```csharp
public void UnMerge()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Объединить ячейки B2 до D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Проверьте, объединена ли ячейка B2 перед разъединением
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Разъединить диапазон
            range.UnMerge();
            
            // Проверьте, объединена ли ячейка B2 после разъединения
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


