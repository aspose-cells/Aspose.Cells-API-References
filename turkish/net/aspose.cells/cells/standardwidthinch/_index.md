---
title: "Cells.StandardWidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Çalışma sayfasındaki varsayılan sütun genişliğini, inç biriminde alır veya ayarlar.

```csharp
public double StandardWidthInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Standart sütun genişliğini inç olarak ayarla
            worksheet.Cells.StandardWidthInch = 1.5;

            // Gösterim için belirli bir sütun genişliğini inç olarak ayarla
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Çalışma kitabını kaydedin
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


