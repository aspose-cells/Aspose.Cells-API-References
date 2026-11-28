---
title: "PivotTable.ShowInCompactForm"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. PivotTable görünümünü kompakt biçimde düzenler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

PivotTable görünümünü kompakt biçimde düzenler.

```csharp
public void ShowInCompactForm()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Kaynak veriden bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Bir pivot tablo çalışma sayfası oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Pivot tablo ekle
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Alanları bölgelere ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot tabloyu kompakt biçimde gösterecek şekilde ayarla
            pivotTable.ShowInCompactForm();
            
            // Verileri hesapla ve yenile
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


