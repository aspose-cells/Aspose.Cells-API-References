---
title: "SubtotalSetting.TotalList"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SubtotalSetting. Массив целочисленных смещений с нулевой базой, указывающих поля, к которым добавляются промежуточные итоги"
type: docs
url: /ru/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Массив смещений полей, начинающихся с нуля, указывающий поля, к которым добавляются промежуточные итоги.

```csharp
public int[] TotalList { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настройка примерных данных
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Создайте и примените промежуточный итог
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Получите настройку промежуточного итога, чтобы продемонстрировать использование TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Сохраните книгу
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### См. также

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


