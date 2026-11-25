---
title: "Enum ViewType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ViewType enum. Rappresenta il tipo di visualizzazione del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/viewtype/
---
## ViewType enumeration

Rappresenta il tipo di visualizzazione del foglio di lavoro.

```csharp
public enum ViewType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il tipo di visualizzazione del foglio di lavoro su PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Salva la cartella di lavoro
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


