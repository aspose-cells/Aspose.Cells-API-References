---
title: "PivotField.Position"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bölgedeki PivotField'ın dizinini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Bölgedeki [`PivotField`](../) dizinini temsil eder.

```csharp
public int Position { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // İlk çalışma sayfasına ve onun pivot tablosuna erişin
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Position özelliğinin kullanımını gösterin
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Rapor filtre sayfalarını göstermek için position'ı kullanın
            pt.ShowReportFilterPageByIndex(position);
            
            // Çalışma kitabını kaydedin
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


