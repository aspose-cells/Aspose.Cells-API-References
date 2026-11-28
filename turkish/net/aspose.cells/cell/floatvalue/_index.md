---
title: "Cell.FloatValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrede bulunan kayan nokta değerini alır"
type: docs
url: /tr/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Hücrede bulunan float değerini alır.

```csharp
public float FloatValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayısal değeri doğrudan ayarlayın
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // Kayan nokta döndüren formülü ayarlayın
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // Paylaşılan formülle FloatValue'yi gösterin
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


