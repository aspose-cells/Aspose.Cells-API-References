---
title: "Cell.DoubleValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrede bulunan çift (double) değeri alır."
type: docs
url: /tr/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Hücrede bulunan double değerini alır.

```csharp
public double DoubleValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelerde farklı değer tiplerini ayarla.
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // DoubleValue özelliğini göster.
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Diğer değer tiplerinin çift (double) olarak okunabildiğini doğrula.
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


