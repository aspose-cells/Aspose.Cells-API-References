---
title: "Cells.StandardHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Bu çalışma sayfasındaki varsayılan satır yüksekliğini, inç biriminde alır veya ayarlar.

```csharp
public double StandardHeightInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Standart yüksekliği inç olarak alın.
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Yeni bir standart yükseklik ayarlayın (1 inç).
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


