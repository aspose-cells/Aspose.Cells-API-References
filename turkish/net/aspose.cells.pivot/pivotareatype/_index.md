---
title: "Enum PivotAreaType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotAreaType enum. PivotTable'ın bir alanını veya yönünü tanımlamak için kullanılan kural tipini gösterir."
type: docs
url: /tr/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

PivotTable'ın bir alanını veya yönünü tanımlamak için kullanılan kural türünü gösterir.

```csharp
public enum PivotAreaType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Pivot alanı yok. |
| Normal | `1` | Bir başlık veya öğeyi temsil eder. |
| Data | `2` | Veri alanındaki bir şeyi temsil eder. |
| All | `3` | Tüm PivotTable'ı temsil eder. |
| Origin | `4` | PivotTable'ın sol üst köşesindeki (RTL sayfalar için sağ üst) boş hücreleri temsil eder. |
| Button | `5` | Bir alan düğmesini temsil eder. |
| TopRight | `6` | PivotTable'ın sağ üst köşesindeki (RTL sayfalar için sol üst) boş hücreleri temsil eder. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Bir PivotTable oluştur
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // PivotTable'a alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // PivotTable için bir PivotArea oluştur
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // PivotArea özelliklerini çıktı olarak ver
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


