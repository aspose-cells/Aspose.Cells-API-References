---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob das Festlegen der QuotePrefix‑Eigenschaft beim Eingeben eines Zeichenfolgenwertes, der mit einem einfachen Anführungszeichen beginnt, in die Zelle"
type: docs
url: /de/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Gibt an, ob das Festlegen der [`QuotePrefix`](../../style/quoteprefix/)-Eigenschaft beim Eingeben des Zeichenfolgenwertes (der mit einem einfachen Anführungszeichen beginnt) in die Zelle

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Beispiele

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
            
            // QuotePrefixToStyle aktivieren – Zeichenketten, die mit ' beginnen, erhalten den QuotePrefix‑Stil
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // QuotePrefixToStyle deaktivieren – Zeichenketten behalten ihren wörtlichen Wert
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

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


