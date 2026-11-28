---
title: "PivotField.Number"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Sayıların ve tarihlerin yerleşik görüntüleme biçimini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Sayıların ve tarihlerin yerleşik görüntüleme biçimini temsil eder.

```csharp
public int Number { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Sütun alanına tarih alanı ekle ve sayı biçimini ayarla
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Özet tabloyu yenile ve hesapla
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


