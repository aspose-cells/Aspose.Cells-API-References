---
title: "PivotField.SortSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Otomatik sıralamanın tüm ayarlarını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

Otomatik sıralamanın tüm ayarlarını alır

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertySortSettingDemo
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
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 75;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];

            // SortSetting özelliğini gösterin
            rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);

            // Sıralama ayarlarını değiştirin
            rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
            Console.WriteLine("\nAfter changing sort settings:");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


