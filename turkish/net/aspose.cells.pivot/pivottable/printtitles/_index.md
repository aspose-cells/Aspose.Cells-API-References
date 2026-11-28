---
title: "PivotTable.PrintTitles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur.

```csharp
public bool PrintTitles { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Pivot tablo alanlarını yapılandırın
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // PrintTitles özelliğini göster
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


