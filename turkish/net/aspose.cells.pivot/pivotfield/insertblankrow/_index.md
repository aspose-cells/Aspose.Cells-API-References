---
title: "PivotField.InsertBlankRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Her öğeden sonra boş bir satır eklenip eklenmeyeceğini gösterir. Yalnızca satır alanları için."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/insertblankrow/
---
## PivotField.InsertBlankRow property

Her öğeden sonra boş bir satır eklenip eklenmeyeceğini gösterir. Yalnızca satır alanları için.

```csharp
public bool InsertBlankRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyInsertBlankRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B5"].Value = 5;
            sheet.Cells["A6"].Value = "Orange";
            sheet.Cells["B6"].Value = 8;
            
            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // InsertBlankRow özelliğini ayarla
            PivotField rowField = pivotTable.RowFields[0];
            rowField.InsertBlankRow = true;
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldInsertBlankRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


