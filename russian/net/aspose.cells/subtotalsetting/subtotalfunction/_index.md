---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SubtotalSetting. Функция промежуточного итога"
type: docs
url: /ru/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

Функция промежуточного итога.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Создайте настройку промежуточного итога, получив её из существующих данных
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Настройте промежуточный итог — эти свойства доступны только для чтения в реальном API
            // Поэтому мы будем использовать метод Subtotal напрямую с параметрами
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Примените промежуточные итоги
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Проверьте свойство SubtotalFunction из полученной настройки
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Сохраните книгу
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


