---
title: "PivotFilter.GetDateTimeValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter yöntemi. Sayı filtresinin değerlerini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/getdatetimevalues/
---
## PivotFilter.GetDateTimeValues method

Numara filtresinin değerlerini alır.

```csharp
public DateTime[] GetDateTimeValues()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetDateTimeValuesDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = DateTime.Now;
            cells["B2"].Value = 1000;
            cells["A3"].Value = DateTime.Now.AddDays(1);
            cells["B3"].Value = 2000;
            cells["A4"].Value = DateTime.Now.AddDays(2);
            cells["B4"].Value = 3000;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Satır alanı ekle ve tarih filtresi uygula
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.BaseFields[0].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
            
            // Filtreyi al ve GetDateTimeValues'i göster
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            DateTime[] dateValues = filter.GetDateTimeValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("First Date Value: " + dateValues[0]);
            Console.WriteLine("Second Date Value: " + dateValues[1]);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


