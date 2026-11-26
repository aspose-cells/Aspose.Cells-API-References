---
title: "SeriesCollection.SetSeriesNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SeriesCollection. Устанавливает имена всех серий на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Задает имена всех серий в диаграмме.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Индекс первой серии, для которой вы хотите установить имя. |
| область | String | Указывает область для имени серии. |
| isVertical | Boolean | &gt;Указывает, следует ли строить серию из диапазона значений ячеек по строкам или по столбцам. |

### Примечания

Если начальный индекс больше количества серий, метод вернётся и ничего не сделает. Если задавать данные в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5. Если задавать данные в смежных ячейках, используйте запятую для их разделения. Например, ($C$2,$D$5).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Получить коллекцию серий диаграммы
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Вызвать SetSeriesNames с параметрами (startIndex: 0, area: "A2:A4", isVertical: true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Добавить данные серии
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


