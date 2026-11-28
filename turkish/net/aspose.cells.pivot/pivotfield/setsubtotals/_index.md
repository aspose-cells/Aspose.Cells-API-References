---
title: "PivotField.SetSubtotals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "**PivotField** yöntemi. Belirtilen alanın alt toplamının nasıl yapılacağını ayarlar."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Belirtilen alanın nasıl alt toplamlanacağını ayarlar.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | [`PivotFieldSubtotalType`](../../pivotfieldsubtotaltype/) |
| gösterildi | Boolean | Belirtilen alanın alt toplamları gösterip göstermediği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            var cells = sheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = "TV";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Electronics";
            cells["B3"].Value = "Radio";
            cells["C3"].Value = 500;
            
            cells["A4"].Value = "Clothing";
            cells["B4"].Value = "Shirt";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "Clothing";
            cells["B5"].Value = "Pants";
            cells["C5"].Value = 400;

            // Pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Satır alanları ekle
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // SetSubtotals'ı PivotFieldSubtotalType ve boolean ile gösterin
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


