---
title: "PivotArea.IsOutline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotArea özelliği. Kuralın, taslak modunda olan bir alana başvurup başvurmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Kuralın, taslak modunda olan bir alana başvurup başvurmadığını gösterir.

```csharp
public bool IsOutline { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // PivotArea oluşturun ve yapılandırın
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


