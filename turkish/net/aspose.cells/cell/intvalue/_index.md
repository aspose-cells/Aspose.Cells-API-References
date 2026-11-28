---
title: "Cell.IntValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrede bulunan tam sayı değerini alır"
type: docs
url: /tr/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Hücrede bulunan tam sayı değerini alır.

```csharp
public int IntValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sayısal bir değer ayarla ve IntValue'yi al
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Sayıya değerlendirilen bir formül ayarla ve IntValue'yi al
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Boolean bir değer ayarla ve IntValue'yi al
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Metin değeri ayarla ve IntValue'yi al (dönüştürülemezse 0 olur)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


