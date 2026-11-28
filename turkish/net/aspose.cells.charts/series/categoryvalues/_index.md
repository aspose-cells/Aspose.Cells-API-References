---
title: "Series.CategoryValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek kategori değerlerini alır"
type: docs
url: /tr/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek kategori değerlerini alır

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Açıklamalar

Bu özellik, özellikle belirtilen veri kaynağı dış bağlantı, formül vb. olduğunda, [`XValues`](../xvalues/) tarafından tanımlanan verilere karşılık gelen gerçek değerleri almanın pratik bir yolunu sunar

### Örnekler

```csharp
//Bu özelliği gerektiren bir durumu göstermek için demo:
[C#]

//Bağımsız örnek
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues, "[External.xlsx]Sheet1!$B$2:$C$6" gibi karmaşık bir şey olabilir
// kullanıcının gerçek değerleri alması için (değerler başka bir çalışma kitabına bağlanmış olabilir,
// veya geçerli çalışma kitabında önbelleğe alınmış olabilir). Burada CategoryValues özelliğini kullanabilirsiniz
// Excel arayüzünde gerçekte görüntülenen kategori değerlerini almak için
// iki boyutlu bir dizi biçiminde.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Ayrıca Bakınız

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


