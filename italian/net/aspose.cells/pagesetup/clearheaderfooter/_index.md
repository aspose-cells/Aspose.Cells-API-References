---
title: "PageSetup.ClearHeaderFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Cancella le impostazioni di intestazione e piè di pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Cancella le impostazioni di intestazione e piè di pagina.

```csharp
public void ClearHeaderFooter()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodClearHeaderFooterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta intestazioni e piè di pagina iniziali
            pageSetup.SetHeader(0, "Initial Left Header");
            pageSetup.SetFooter(0, "Initial Left Footer");

            Console.WriteLine("Before ClearHeaderFooter:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));

            // Cancella intestazioni e piè di pagina
            pageSetup.ClearHeaderFooter();

            Console.WriteLine("\nAfter ClearHeaderFooter:");
            Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
            Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));

            // Imposta nuove intestazioni e piè di pagina dopo la cancellazione
            pageSetup.SetHeader(0, "New Left Header");
            pageSetup.SetFooter(0, "New Left Footer");

            Console.WriteLine("\nAfter Setting New Values:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


