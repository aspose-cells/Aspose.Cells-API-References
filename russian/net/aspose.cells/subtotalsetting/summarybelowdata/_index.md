---
title: "SubtotalSetting.SummaryBelowData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SubtotalSetting. Указывает, следует ли добавлять сводку под данными"
type: docs
url: /ru/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Указывает, следует ли добавить сводку ниже данных.

```csharp
public bool SummaryBelowData { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Создайте область ячеек для промежуточных итогов
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // Примените промежуточные итоги, используя метод Cells.Subtotal со всеми необходимыми параметрами
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // Получите настройку, чтобы проверить SummaryBelowData
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Выведите значение свойства SummaryBelowData
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### См. также

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


