---
title: "SeriesCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. Series koleksiyonunu bir grafiğe ekler"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Bir grafiğe [`Series`](../../series/) koleksiyonunu ekler.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataArea | String | Veri serisini çizecek değerleri belirtir |
| isVertical | Boolean | Serileri hücre değerleri aralığından satır veya sütun bazında çizmeyi belirler. Doğruysa, [`Series`](../../series/) sütun sütun eklenecektir. |

### Dönüş Değeri

Eklenen ASeries'in NSeries içindeki ilk indeksini döndürür.

### Açıklamalar

Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üst üste kullanın. Örneğin, $C$2:$C$5. Ayrık hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin: ($C$2,$D$5). Bu yöntem yalnızca *dataArea*'yı veri aralığı olarak basitçe işler. Akıllıca ChartCollection.Add() yöntemini kontrol etmek istiyorsanız.

### Örnekler

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
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Dize ve boolean parametreleri kullanarak seri ekleyin
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Bir grafiğe [`Series`](../../series/) koleksiyonunu ekler.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | String | Veri serisini çizecek değerleri belirtir |
| isVertical | Boolean | Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| checkLabels | Boolean | Aralığın serinin adını içerip içermediğini gösterir |

### Dönüş Değeri

Eklenen ASeries'in NSeries içindeki ilk indeksini döndürür.

### Açıklamalar

Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üst üste kullanın. Örneğin, $C$2:$C$5. Ayrık hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin, ($C$2,$D$5).

### Örnekler

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
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Dize ve boolean parametreleriyle Add metodunu kullanarak seri ekleyin
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Çalışma kitabını kaydedin
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


