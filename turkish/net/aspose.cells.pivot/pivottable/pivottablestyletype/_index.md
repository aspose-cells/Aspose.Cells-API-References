---
title: "PivotTable.PivotTableStyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Yerleşik pivot tablo stilini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Yerleşik pivot tablo stilini alır ve ayarlar.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTableStyleType'ı ayarla ve göster
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableStyleTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


