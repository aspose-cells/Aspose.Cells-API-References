---
title: "StyleFlag.QuotePrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Hide-Formel-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Die Einstellung zum Ausblenden von Formeln wird angewendet.

```csharp
public bool QuotePrefix { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf Zelle A1 zu und setzen Sie einen Wert, der wie eine Zahl aussieht, aber als Text behandelt werden soll
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Erstellen Sie einen Stil und setzen Sie QuotePrefix auf true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Erstellen Sie ein Style-Flag und aktivieren Sie das QuotePrefix-Flag
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Wenden Sie den Stil auf die Zelle mit SetStyle anstelle von ApplyStyle an
            cell.SetStyle(style, flag);

            // Zeigen Sie den aktuellen QuotePrefix-Wert an
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen (der Wert wird in Excel als Text behandelt)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Jetzt ändern wir QuotePrefix auf false und sehen den Unterschied
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Speichern Sie erneut unter einem anderen Namen zum Vergleich
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


