---
title: "WorkbookSettings.MaxColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar det maximala kolumnindexet, nollbaserat"
type: docs
url: /sv/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Hämtar det maximala kolumnindexet, nollbaserat.

```csharp
public int MaxColumn { get; }
```

### Anmärkningar

Returnerar 255 om filformatet är Excel97-2003;

### Exempel

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
            
            // Demonstrera användning av MaxColumn genom att försöka komma åt en kolumn utanför gränsen
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

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


