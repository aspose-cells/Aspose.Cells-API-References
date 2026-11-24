---
title: "Cells.StandardWidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Standardspaltenbreite im Arbeitsblatt in Zoll zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zoll.

```csharp
public double StandardWidthInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Standardspaltenbreite in Zoll festlegen
            worksheet.Cells.StandardWidthInch = 1.5;

            // Spezifische Spaltenbreite in Zoll für die Demonstration festlegen
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Speichere die Arbeitsmappe
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


