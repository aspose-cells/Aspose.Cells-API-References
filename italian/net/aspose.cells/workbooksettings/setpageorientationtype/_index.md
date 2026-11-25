---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookSettings. Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Il tipo di orientamento della pagina |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Imposta l'orientamento della pagina su Portrait per tutti i fogli di lavoro
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Verifica che l'orientamento sia impostato correttamente
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Vedi anche

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


