---
title: "Worksheet.ShowFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir."
type: docs
url: /tr/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir.

```csharp
public bool ShowFormulas { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine formül ayarla
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Başlangıçta hesaplanmış değeri göster
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Formül metnini göstermek için değiştir
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


