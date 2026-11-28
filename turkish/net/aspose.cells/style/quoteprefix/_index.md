---
title: "Style.QuotePrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücre değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir"
type: docs
url: /tr/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir.

```csharp
public bool QuotePrefix { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B10 hücresine erişin ve değerini ayarlayın
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Hücrenin stilini al ve QuotePrefix'i etkinleştir
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // QuotePrefix özelliğini doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


