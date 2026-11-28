---
title: "PivotArea.PivotArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotArea yapıcı. PivotTable'ın seçili alanını sunar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

PivotTable'ın seçilen alanını sunar.

```csharp
public PivotArea(PivotTable table)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | PivotTable |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
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
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // PivotTable parametresiyle PivotArea yapıcısını göster
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Pivot alanını yapılandır
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


