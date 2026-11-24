---
title: "WorkbookSettings.MaxColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt den maximalen Spaltenindex (nullbasiert) zurück"
type: docs
url: /de/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Liest den maximalen Spaltenindex, nullbasiert.

```csharp
public int MaxColumn { get; }
```

### Hinweise

Gibt 255 zurück, wenn das Dateiformat Excel97-2003 ist;

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Console.WriteLine("MaxColumn value: " + workbook.Settings.MaxColumn);
            
            // Demonstriere die Verwendung von MaxColumn, indem versucht wird, auf eine Spalte jenseits des Limits zuzugreifen
            try
            {
                Cells cells = workbook.Worksheets[0].Cells;
                Cell cell = cells[0, workbook.Settings.MaxColumn + 1];
                Console.WriteLine("This should not be reached");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxColumn: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


