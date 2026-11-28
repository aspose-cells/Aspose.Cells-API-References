---
title: "PivotTable.Indent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Sıkıştırılmış eksen için girinti artışını belirtir ve Rapor Düzeni'ni Sıkıştırılmış Formata ayarlamak için kullanılabilir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir.

```csharp
public int Indent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
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

            // Girinti özelliğini ayarla
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


