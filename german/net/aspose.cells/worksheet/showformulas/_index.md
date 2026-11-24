---
title: "Worksheet.ShowFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden"
type: docs
url: /de/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Gibt an, ob Formeln oder deren Ergebnisse angezeigt werden sollen.

```csharp
public bool ShowFormulas { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Formel in Zelle A1 setzen
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Zunächst berechneten Wert anzeigen
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Umschalten, um Formeltext anzuzeigen
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


