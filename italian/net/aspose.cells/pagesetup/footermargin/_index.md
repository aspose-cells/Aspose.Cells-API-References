---
title: "PageSetup.FooterMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta la distanza dal fondo della pagina al piè di pagina in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Rappresenta la distanza dal bordo inferiore della pagina al piè di pagina, in unità di centimetri.

```csharp
public double FooterMargin { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta il margine del piè di pagina in centimetri
            pageSetup.FooterMargin = 1.5;

            // Aggiungi del contenuto per vedere l'effetto
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Imposta il testo del piè di pagina per rendere visibile il margine
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Salva la cartella di lavoro
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


