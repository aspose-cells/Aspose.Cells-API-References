---
title: "Hyperlink.Address"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑egenskap. Representerar adressen för en hyperlänk"
type: docs
url: /sv/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Representerar adressen för en hyperlänk.

```csharp
public string Address { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till hyperlänkar med olika adresser
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Åtkomst till och visning av hyperlänkadresser
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Spara arbetsboken
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


