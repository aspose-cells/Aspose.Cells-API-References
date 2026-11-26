---
title: "Series.PointValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает фактические значения, используемые для построения каждой точки этой серии в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Получает фактические значения, используемые для построения каждой точки этого ряда на диаграмме.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Примечания

Это свойство предоставляет удобный способ получить фактические значения, соответствующие данным, определённым с помощью [`Values`](../values/), особенно когда указанный источник данных является внешней ссылкой, формулой и т.д.

### Примеры

```csharp
//Пример, показывающий случай, требующий этого свойства:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Values может выглядеть как "[External.xlsx]Sheet1!$A$1:$A$6", что является сложным
// для пользователя, чтобы получить фактические значения (значения могут быть связаны с другой книгой,
// или кэшированы в текущей книге). Здесь можно использовать свойство PointValues
// чтобы получить значения, действительно отображаемые в интерфейсе Excel
// в виде массива.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### См. также

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


