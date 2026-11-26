---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. Indica si se establece la propiedad QuotePrefix al ingresar el valor de cadena que comienza con una comilla simple en la celda"
type: docs
url: /es/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Indica si al establecer la propiedad [`QuotePrefix`](../../style/quoteprefix/) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Ejemplos

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
            
            // Activar QuotePrefixToStyle - las cadenas que comienzan con ' tendrán aplicado el estilo QuotePrefix
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // Desactivar QuotePrefixToStyle - las cadenas conservan su valor literal
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

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


