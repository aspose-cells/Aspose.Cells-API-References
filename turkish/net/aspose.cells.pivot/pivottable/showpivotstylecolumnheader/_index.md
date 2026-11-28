---
title: "PivotTable.ShowPivotStyleColumnHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Pivot tablo içindeki sütun başlığının stile uygulanıp uygulanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showpivotstylecolumnheader/
---
## PivotTable.ShowPivotStyleColumnHeader property

Pivot tablo içindeki sütun başlığının stile uygulanıp uygulanmayacağını gösterir.

```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnHeaderDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Bir pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Pivot tablo stilini ayarla
            pivotTable.ShowPivotStyleColumnHeader = true;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableShowPivotStyleColumnHeaderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


