---
title: "WorkbookSettings.MaxRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar det maximala radindexet, nollbaserat"
type: docs
url: /sv/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Hämtar det maximala radindexet, nollbaserat.

```csharp
public int MaxRow { get; }
```

### Anmärkningar

Returnerar 65535 om filformatet är Excel97-2003;

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Demonstrera MaxRow-egenskapen
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Försök att komma åt en cell utanför MaxRow (ska kasta ett undantag)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Skapa ett cellområde med hjälp av MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


