---
title: "PivotField.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. PivotField adını temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/name/
---
## PivotField.Name property

PivotField adını temsil eder.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNameDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2024, 1, 5);
            sheet.Cells["A3"].Value = new DateTime(2024, 1, 10);
            sheet.Cells["A4"].Value = new DateTime(2024, 2, 15);
            sheet.Cells["A5"].Value = new DateTime(2024, 3, 20);
            
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;
            sheet.Cells["B5"].Value = 400;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Satır alanı ekleyin ve Name özelliğini gösterin
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.RowFields[0].Name = "MyDateField";
            
            // Aylar ve yıllara göre gruplayın
            DateTime start = new DateTime(2024, 1, 1);
            DateTime end = new DateTime(2024, 12, 31);
            pt.RowFields[0].GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, true);
            
            // Gruplanmış alanların adlarını çıkartın
            Console.WriteLine("Row Field 0 Name: " + pt.RowFields[0].Name); // Will show "MyYears"
            Console.WriteLine("Row Field 1 Name: " + pt.RowFields[1].Name); // Will show "MyMonths"
            
            // Çalışma kitabını kaydedin
            wb.Save("PivotFieldNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


