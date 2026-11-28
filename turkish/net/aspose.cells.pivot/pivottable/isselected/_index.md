---
title: "PivotTable.IsSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bu PivotTable'ın seçili olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Bu **PivotTable**'ın seçili olup olmadığını gösterir.

```csharp
public bool IsSelected { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
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
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Başlangıçta, IsSelected false'tur
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Pivot tabloyu seç
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Pivot tablo seçimini kaldır
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


