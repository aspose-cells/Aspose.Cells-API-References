---
title: "SubtotalSetting.GroupBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SubtotalSetting. Поле для группировки в виде целочисленного смещения с нулевой базой"
type: docs
url: /ru/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Поле для группировки, как целочисленное смещение, начинающееся с нуля

```csharp
public int GroupBy { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Group A");
            worksheet.Cells["A3"].PutValue("Group B");
            worksheet.Cells["A4"].PutValue("Group A");
            worksheet.Cells["A5"].PutValue("Group B");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);

            try
            {
                // Определите область ячеек для промежуточных итогов
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Примените промежуточные итоги к данным
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Получите настройку subtotal, чтобы получить доступ к свойству GroupBy
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Отобразите значение свойства GroupBy
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Сохраните книгу
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


