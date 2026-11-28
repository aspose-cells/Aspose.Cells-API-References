---
title: "PivotField.Ungroup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Pivot alanını gruptan çıkar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Pivot alanının grubunu kaldır.

```csharp
public void Ungroup()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // İlk sütun alanını gruptan çıkar
            pivotTable.ColumnFields[0].Ungroup();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


