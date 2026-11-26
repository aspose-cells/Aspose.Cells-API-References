---
title: "SeriesCollection.ChangeSeriesOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SeriesCollection. Непосредственно изменяет порядок двух рядов"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/changeseriesorder/
---
## SeriesCollection.ChangeSeriesOrder method

Непосредственно изменяет порядок двух серий.

```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceIndex | Int32 | Текущий индекс |
| destIndex | Int32 | Индекс назначения |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод SeriesCollection.SwapSeries. Этот метод будет удалён через 12 месяцев, начиная с июня 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodChangeSeriesOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(60);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(70);
            worksheet.Cells["C3"].PutValue(80);
            worksheet.Cells["C4"].PutValue(90);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            
            // Получите коллекцию серий
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Вызовите метод ChangeSeriesOrder, чтобы поменять местами ряды с индексами 0 и 2
                seriesCollection.ChangeSeriesOrder(0, 2);
                
                Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
                
                // Отобразите новый порядок рядов
                for (int i = 0; i < seriesCollection.Count; i++)
                {
                    Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


