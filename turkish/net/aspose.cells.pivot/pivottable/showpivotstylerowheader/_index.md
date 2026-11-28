---
title: "PivotTable.ShowPivotStyleRowHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Pivot tabloda satır başlığının stilinin uygulanıp uygulanmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showpivotstylerowheader/
---
## PivotTable.ShowPivotStyleRowHeader property

Pivot tablo içindeki satır başlığının stile uygulanıp uygulanmayacağını gösterir.

```csharp
public bool ShowPivotStyleRowHeader { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowHeaderDemo
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

            // ShowPivotStyleRowHeader özelliğini göster
            pivotTable.ShowPivotStyleRowHeader = true;
            Console.WriteLine("ShowPivotStyleRowHeader is set to: " + pivotTable.ShowPivotStyleRowHeader);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableShowPivotStyleRowHeaderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


