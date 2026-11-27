---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger om inställning av QuotePrefix-egenskapen när ett strängvärde som börjar med enkelfnutt matas in i cellen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Anger om inställning av [`QuotePrefix`](../../style/quoteprefix/) egenskapen när ett strängvärde (som börjar med enkelfnutt) matas in i cellen

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Exempel

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
            
            // Aktivera QuotePrefixToStyle – strängar som börjar med ' får QuotePrefix-stil tillämpad
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // Inaktivera QuotePrefixToStyle – strängar behåller sitt bokstavliga värde
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

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


