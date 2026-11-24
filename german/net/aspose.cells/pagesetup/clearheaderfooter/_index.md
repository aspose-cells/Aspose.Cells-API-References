---
title: "PageSetup.ClearHeaderFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Löscht die Kopf- und Fußzeileneinstellung"
type: docs
url: /de/net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Löscht die Kopf- und Fußzeileneinstellungen.

```csharp
public void ClearHeaderFooter()
```

### Beispiele

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

            // Initiale Kopf- und Fußzeilen festlegen
            pageSetup.SetHeader(0, "Initial Left Header");
            pageSetup.SetFooter(0, "Initial Left Footer");

            Console.WriteLine("Before ClearHeaderFooter:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));

            // Kopf- und Fußzeilen löschen
            pageSetup.ClearHeaderFooter();

            Console.WriteLine("\nAfter ClearHeaderFooter:");
            Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
            Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));

            // Neue Kopf- und Fußzeilen nach dem Löschen festlegen
            pageSetup.SetHeader(0, "New Left Header");
            pageSetup.SetFooter(0, "New Left Footer");

            Console.WriteLine("\nAfter Setting New Values:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


