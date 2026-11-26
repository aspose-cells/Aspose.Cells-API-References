---
title: "Класс SubtotalSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SubtotalSetting. Представляет настройки промежуточного итога"
type: docs
url: /ru/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Представляет настройку промежуточного итога .

```csharp
public class SubtotalSetting
```

## Свойства

| Имя | Описание |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | Поле для группировки, как целочисленное смещение, начинающееся с нуля |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | Функция промежуточного итога. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Указывает, следует ли добавить сводку ниже данных. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | Массив смещений полей, начинающихся с нуля, указывающий поля, к которым добавляются промежуточные итоги. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить примерные данные в лист
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

                // Получите объект SubtotalSetting из листа
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Отобразите свойства объекта SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Сохраните книгу
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


