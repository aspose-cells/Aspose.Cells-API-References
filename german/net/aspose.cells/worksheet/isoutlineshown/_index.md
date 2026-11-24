---
title: "Worksheet.IsOutlineShown"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet‑Eigenschaft. Gibt an, ob die Gliederung angezeigt werden soll"
type: docs
url: /de/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Gibt an, ob die Gliederung angezeigt werden soll.

```csharp
public bool IsOutlineShown { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Legen Sie fest, dass die Gliederung angezeigt wird
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Speichern und neu laden, um die Persistenz zu demonstrieren
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


