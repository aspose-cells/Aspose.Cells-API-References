---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable'ı yenilerken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir; true ise bir dize 255 karakterden az veya eşit olmalıdır, 255 karakterden uzun ise kesilir. false ise dize bu sınırlamaya tabi değildir. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

PivotTable yenilenirken **PivotTable**'ın Excel2003 ile uyumlu olup olmadığını belirtir; true ise bir dize 255 karakterden az veya eşit olmalıdır, 255 karakterden uzun ise kesilir. false ise dize bu sınırlamaya tabi değildir. Varsayılan değer true'tur.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Bir çalışma sayfası ekle ve örnek veri ile doldur
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Örnek veri satırları ekle
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Bir pivot tablo ekle
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Pivot tablo alanlarını yapılandırın
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Uyumluluk modunu ayarla
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Verileri yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


