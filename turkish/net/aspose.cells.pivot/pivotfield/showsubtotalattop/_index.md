---
title: "PivotField.ShowSubtotalAtTop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir.

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Açıklamalar

Yalnızca ShowInOutlineForm true olduğunda satır bölgesindeki pivot alanları için çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Satır alanı ekle ve alt toplam konumunu yapılandır
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


