---
title: "SeriesCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SeriesCollection. Добавляет коллекцию Series к диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Добавляет коллекцию [`Series`](../../series/) к диаграмме.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataArea | String | Указывает значения, из которых строится серия данных |
| isVertical | Boolean | Указывает, следует ли строить серию из диапазона значений ячеек по строкам или по столбцам. Если true, [`Series`](../../series/) будет добавлен столбец за столбцом |

### Возвращаемое значение

Возвращает первый индекс добавленного ASeries в NSeries.

### Примечания

Если данные задаются в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5. Если данные задаются в несмежных ячейках, используйте запятую для их разделения. Например: ($C$2,$D$5). Этот метод просто обрабатывает *dataArea* как диапазон данных. Если вы хотите интеллектуально проверить метод ChartCollection.Add().

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Добавьте серию, используя строковые и логические параметры
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Сохраните книгу
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Добавляет коллекцию [`Series`](../../series/) к диаграмме.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | String | Указывает значения, из которых строится серия данных |
| isVertical | Boolean | Указывает, строить ли серию из диапазона ячеек по строкам или по столбцам. |
| checkLabels | Boolean | Указывает, содержит ли диапазон имя серии |

### Возвращаемое значение

Возвращает первый индекс добавленного ASeries в NSeries.

### Примечания

Если данные задаются в смежных ячейках, используйте двоеточие для их разделения. Например, $C$2:$C$5. Если данные задаются в несмежных ячейках, используйте запятую для их разделения. Например, ($C$2,$D$5).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Добавьте серию, используя метод Add со строковыми и логическими параметрами
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Сохраните книгу
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


