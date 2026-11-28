---
title: "Cell.BoolValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrede bulunan boolean değeri alır"
type: docs
url: /tr/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Hücrede bulunan boolean değeri alır.

```csharp
public bool BoolValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Boolean değere değerlendiren bir formül ayarla
            cell.Formula = "=2.01>2";
            
            // Sonucu elde etmek için formülü hesapla
            workbook.CalculateFormula();
            
            // BoolValue özelliğini göster
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


