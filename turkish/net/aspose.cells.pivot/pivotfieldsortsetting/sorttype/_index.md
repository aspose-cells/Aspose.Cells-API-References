---
title: "PivotFieldSortSetting.SortType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldSortSetting özelliği. SortOrder'ı temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Şu [`SortOrder`](../../../aspose.cells/sortorder/) öğesini temsil eder.

```csharp
public SortOrder SortType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertySortTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Satır alanını artan sırada sırala
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
            
            // SortType özelliğini göster
            Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Sıralama düzenini değiştir ve tekrar göster
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
            Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


