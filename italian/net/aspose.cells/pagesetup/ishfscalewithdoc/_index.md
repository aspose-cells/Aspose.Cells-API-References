---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Indica se intestazione e piè di pagina sono scalati con la scala del documento. Si applica solo a Excel 2007"
type: docs
url: /it/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Indica se intestazione e piè di pagina sono scalati con la scala del documento. Valido solo per Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta la configurazione di pagina di base
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Dimostra la proprietà IsHFScaleWithDoc
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


