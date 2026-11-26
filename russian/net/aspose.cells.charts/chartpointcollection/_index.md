---
title: "Класс ChartPointCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartPointCollection. Представляет коллекцию, содержащую все точки в одной серии"
type: docs
url: /ru/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Представляет коллекцию, содержащую все точки в одной серии.

```csharp
public class ChartPointCollection : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Получает количество точек диаграммы. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Получает элемент [`ChartPoint`](../chartpoint/) по указанному индексу в серии. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Удалить все настройки точек диаграммы. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Возвращает перечислитель для всей `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Удаляет точку по индексу серии. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];

            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Показать подписи данных 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Доступ к ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Итерация по точкам в коллекции
            for (int i = 0; i < points.Count; i++)
            {
                // Получить точку данных
                ChartPoint point = points[i];
                
                // Установить взрыв круговой диаграммы
                point.Explosion = 15;
                
                // Установить цвет границы
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Сохранение файла Excel
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


