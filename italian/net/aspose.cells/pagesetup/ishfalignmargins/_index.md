---
title: "PageSetup.IsHFAlignMargins"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. Se questa proprietà è true, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro e l'intestazione e il piè di pagina destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita"
type: docs
url: /it/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. Se questa proprietà è true, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro, e quelli destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta IsHFAlignMargins a true
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Modifica IsHFAlignMargins a false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


