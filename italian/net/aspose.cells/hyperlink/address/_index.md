---
title: "Hyperlink.Address"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Hyperlink. Rappresenta l'indirizzo di un collegamento ipertestuale"
type: docs
url: /it/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Rappresenta l'indirizzo di un hyperlink.

```csharp
public string Address { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi collegamenti ipertestuali con indirizzi diversi
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Accedi e visualizza gli indirizzi dei collegamenti ipertestuali
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Salva la cartella di lavoro
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


