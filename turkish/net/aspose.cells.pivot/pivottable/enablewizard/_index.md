---
title: "PivotTable.EnableWizard"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable Sihirbazının mevcut olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

**PivotTable Wizard**'ın mevcut olup olmadığını gösterir.

```csharp
public bool EnableWizard { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableWizardDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // Pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTable sihirbazını devre dışı bırak
            pivotTable.EnableWizard = false;

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


