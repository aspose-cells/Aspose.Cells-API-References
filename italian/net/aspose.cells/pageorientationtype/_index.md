---
title: "Enum PageOrientationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.PageOrientationType. Rappresenta le costanti di orientamento di stampa"
type: docs
url: /it/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Rappresenta le costanti di orientamento di stampa.

```csharp
public enum PageOrientationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Landscape | `0` | Orientamento orizzontale |
| Portrait | `1` | Orientamento verticale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi all'oggetto PageSetup del foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta l'orientamento della pagina su Landscape
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Salva la cartella di lavoro in un file
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Imposta l'orientamento della pagina su Portrait
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Salva la cartella di lavoro in un file diverso
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


