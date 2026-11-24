---
title: "WorkbookSettings.MaxRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt den maximalen Zeilenindex zurück, nullbasiert"
type: docs
url: /de/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Liest den maximalen Zeilenindex, nullbasiert.

```csharp
public int MaxRow { get; }
```

### Hinweise

Gibt 65535 zurück, wenn das Dateiformat Excel97-2003 ist;

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // MaxRow-Eigenschaft demonstrieren
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Versuchen Sie, auf eine Zelle jenseits von MaxRow zuzugreifen (sollte eine Ausnahme auslösen)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Erstellen Sie einen Zellbereich unter Verwendung von MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


