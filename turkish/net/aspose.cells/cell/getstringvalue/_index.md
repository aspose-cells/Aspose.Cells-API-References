---
title: "Cell.GetStringValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell method. Belirli bir biçimlendirme stratejisiyle dize değerini alır."
type: docs
url: /tr/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Belirli bir biçimlendirme stratejisiyle dize değerini al.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | Biçimlendirilmiş strateji. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelerde farklı veri türleri ayarla
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // GetStringValue'i farklı biçimlendirme stratejileriyle göster
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


