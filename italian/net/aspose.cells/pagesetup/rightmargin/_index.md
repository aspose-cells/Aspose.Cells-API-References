---
title: "PageSetup.RightMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine destro in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Rappresenta la dimensione del margine destro, in centimetri.

```csharp
public double RightMargin { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta margini destro diversi e salva per dimostrare l'effetto
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Stampa il valore corrente del margine destro
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


