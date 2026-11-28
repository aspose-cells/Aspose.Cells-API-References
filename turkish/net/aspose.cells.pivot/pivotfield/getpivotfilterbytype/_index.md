---
title: "PivotField.GetPivotFilterByType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Pivot alanının tipine göre pivot filtresini alır."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

Pivot alanının tipine göre pivot filtresini alır

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            
            sheet.Cells["B1"].Value = "Count";
            sheet.Cells["B2"].Value = 1;
            sheet.Cells["B3"].Value = 2;
            sheet.Cells["B4"].Value = 3;
            sheet.Cells["B5"].Value = 4;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Sayım filtresini uygula
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Sayım filtresini al
            PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
            
            // Filtre ayrıntılarını çıktıla
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            Console.WriteLine("Auto Filter: " + filter.AutoFilter);
            
            wb.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


