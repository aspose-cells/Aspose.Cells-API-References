---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Tek tırnak işaretiyle başlayan dize değerini hücreye girerken QuotePrefix özelliğinin ayarlanıp ayarlanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Tek tırnak işaretiyle başlayan dize değerini hücreye girerken [`QuotePrefix`](../../style/quoteprefix/) özelliğinin ayarlanıp ayarlanmadığını gösterir

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyQuotePrefixToStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // QuotePrefixToStyle'ı etkinleştir - ' ile başlayan dizeler QuotePrefix stiline sahip olur
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // QuotePrefixToStyle'ı devre dışı bırak - dizeler gerçek değerlerini korur
            workbook.Settings.QuotePrefixToStyle = false;
            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.PutValue("'abc");
            Console.WriteLine("Cell A2 - QuotePrefix: " + cell2.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A2 - Value: " + cell2.StringValue);

            workbook.Save("QuotePrefixToStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


