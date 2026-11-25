---
title: "Worksheet.IsPageBreakPreview"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se il foglio di lavoro specificato è visualizzato nella vista normale o nell'anteprima interruzione di pagina"
type: docs
url: /it/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Indica se il foglio di lavoro specificato è mostrato nella visualizzazione normale o nell'anteprima interruzione di pagina.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il foglio di lavoro in modalità Anteprima interruzione di pagina
            worksheet.IsPageBreakPreview = true;
            
            // Imposta lo zoom al 100% per la dimostrazione
            worksheet.Zoom = 100;
            
            // Restituisci le impostazioni correnti
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


