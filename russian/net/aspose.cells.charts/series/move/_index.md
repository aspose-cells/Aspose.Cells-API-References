---
title: "Series.Move"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Series. Перемещает серию вверх или вниз"
type: docs
url: /ru/net/aspose.cells.charts/series/move/
---
## Series.Move method

Перемещает ряд вверх или вниз.

```csharp
public void Move(int count)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| количество | Int32 | Количество перемещений вверх или вниз. Переместите серию вверх, если значение меньше нуля; переместите серию вниз, если значение больше нуля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Получить первую серию
            Series series = chart.NSeries[0];
            
            try
            {
                // Вызовите метод Move с параметром Int32
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Покажите эффект, изменив имя серии
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


