---
title: "Series.CategoryValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает фактические значения категорий, которые используются для построения каждой точки этой серии на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Получает фактические значения категорий, используемые для построения каждой точки этой серии в диаграмме.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Примечания

Это свойство предоставляет удобный способ получить фактические значения, соответствующие данным, определённым с помощью [`XValues`](../xvalues/), особенно когда указанный источник данных является внешней ссылкой, формулой и т.д.

### Примеры

```csharp
//Пример, показывающий случай, требующий этого свойства:
[C#]

//Отдельный пример
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues может выглядеть как "[External.xlsx]Sheet1!$B$2:$C$6", что сложно
// для пользователя, чтобы получить фактические значения (значения могут быть связаны с другой книгой,
// или кэшировано в текущей рабочей книге). Здесь вы можете использовать свойство CategoryValues
// чтобы получить значения категорий, фактически отображаемые в интерфейсе Excel
// в виде двумерного массива.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### См. также

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


