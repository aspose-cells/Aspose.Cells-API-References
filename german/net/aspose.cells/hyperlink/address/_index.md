---
title: "Hyperlink.Address"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Hyperlink-Eigenschaft. Stellt die Adresse eines Hyperlinks dar"
type: docs
url: /de/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Stellt die Adresse eines Hyperlinks dar.

```csharp
public string Address { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hyperlinks mit unterschiedlichen Adressen hinzufügen
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Auf Hyperlink-Adressen zugreifen und sie anzeigen
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


