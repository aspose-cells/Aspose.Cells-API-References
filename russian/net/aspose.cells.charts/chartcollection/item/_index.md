---
title: "ChartCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartCollection. Возвращает элемент Chart по указанному индексу"
type: docs
url: /ru/net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

Возвращает элемент [`Chart`](../../chart/) по указанному индексу.

```csharp
public Chart this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            
            // Получить доступ к диаграмме с помощью свойства Item
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить источник данных диаграммы и заголовок
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Title.Text = "Sample Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Chart created successfully with Item property access.");
        }
    }
}
```

### См. также

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

Возвращает диаграмму по имени.

```csharp
public Chart this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя диаграммы. |

### Возвращаемое значение

Диаграмма.

### Примечания

Имя диаграммы по умолчанию равно null. Поэтому вам необходимо явно задать имя диаграммы.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Добавить диаграмму в лист
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);

                // Получите доступ к диаграмме, используя свойство Item (индексатор)
                Chart chart = worksheet.Charts[chartIndex];

                // Отобразить информацию о диаграмме
                Console.WriteLine("Chart type: " + chart.Type);
                Console.WriteLine("Chart name: " + chart.Name);

                // Сохраните книгу
                workbook.Save("ChartCollectionItemDemo.xlsx");

                Console.WriteLine("Chart created and accessed successfully using Item property.");
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

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


