---
title: "PageSetup.IsPercentScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come viene scalato il foglio di lavoro"
type: docs
url: /it/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro viene scalato.

```csharp
public bool IsPercentScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup e imposta la scala all'80% (scala percentuale)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Emetti le impostazioni per dimostrare IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


