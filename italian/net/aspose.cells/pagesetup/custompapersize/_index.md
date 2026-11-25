---
title: "PageSetup.CustomPaperSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta le dimensioni personalizzate della carta nell'unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Imposta la dimensione personalizzata della carta, in pollici.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| larghezza | Double | La larghezza della carta. |
| altezza | Double | L'altezza della carta. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le dimensioni personalizzate della carta (larghezza: 1,5 pollici, altezza: 1,5 pollici)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Salva la cartella di lavoro per dimostrare l'effetto
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


