---
title: "Sınıf PivotTableFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTableFormat sınıfı. PivotTable içinde tanımlanan biçimi temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

PivotTable içinde tanımlanan biçimi temsil eder.

```csharp
public class PivotTableFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Pivot alanını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Biçimlendirilmiş stili alır. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Pivot alanının stilini ayarlar. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Bir pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // PivotTableFormatCollection'a eriş
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Koleksiyona yeni bir biçim ekle
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Biçimin PivotArea'sına erişin
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Yeni bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Stili PivotTableFormat'a uygulayın
            pivotFormat.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


