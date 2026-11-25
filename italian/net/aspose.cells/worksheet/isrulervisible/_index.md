---
title: "Worksheet.IsRulerVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se il righello è visibile. Questa proprietà è applicata solo per l'anteprima interruzione di pagina"
type: docs
url: /it/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Indica se il righello è visibile. Questa proprietà è applicata solo per l'anteprima interruzione di pagina.

```csharp
public bool IsRulerVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta il foglio di lavoro su PageLayoutView dove il righello è visibile
            worksheet.ViewType = ViewType.PageLayoutView;

            // Attiva/disattiva la visibilità del righello
            worksheet.IsRulerVisible = true;

            // Restituisci lo stato attuale della visibilità del righello
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Salva la cartella di lavoro
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


