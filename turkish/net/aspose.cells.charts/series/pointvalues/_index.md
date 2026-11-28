---
title: "Series.PointValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek değerleri alır"
type: docs
url: /tr/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek değerleri alır.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Açıklamalar

Bu özellik, özellikle belirtilen veri kaynağı dış bağlantı, formül vb. olduğunda, [`Values`](../values/) ile tanımlanan verilere karşılık gelen gerçek değerleri almanın pratik bir yolunu sunar.

### Örnekler

```csharp
//Bu özelliği gerektiren bir durumu göstermek için demo:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Values, "[External.xlsx]Sheet1!$A$1:$A$6" gibi karmaşık bir şey olabilir
// kullanıcının gerçek değerleri alması için (değerler başka bir çalışma kitabına bağlanmış olabilir,
// veya mevcut çalışma kitabında önbelleğe alınmış olabilir). Burada PointValues özelliğini kullanabilirsiniz
// Excel arayüzünde gerçekte görüntülenen değerleri almak için
// dizi biçiminde.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Ayrıca Bakınız

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


