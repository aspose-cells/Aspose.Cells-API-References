---
title: "PivotTable.RowHeaderCaption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bu PivotTable'taki Satır Başlığının özel başlığını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Bu PivotTable'daki Satır Başlığının özel başlığını alır ve ayarlar.

```csharp
public string RowHeaderCaption { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Veri çalışma sayfası ekle
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Örnek veri ekleyin.
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Pivot tablo çalışma sayfası ekle
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Pivot tablo ekle ve indeksini al
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Pivot tablo örneğini al
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Pivot tabloyu yapılandır
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


