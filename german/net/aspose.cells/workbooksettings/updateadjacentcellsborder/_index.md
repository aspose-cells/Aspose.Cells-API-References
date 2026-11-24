---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Ränder benachbarter Zellen aktualisiert werden"
type: docs
url: /de/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Gibt an, ob die Ränder angrenzender Zellen aktualisiert werden.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Hinweise

Der Standardwert ist false. Zum Beispiel: Der untere Rand der Zelle A1 wird aktualisiert, der obere Rand der Zelle A2 sollte ebenfalls geändert werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Aktivieren Sie die Aktualisierung der Ränder benachbarter Zellen
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Wert setzen und Rand auf Zelle A1 anwenden
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Wert in benachbarte Zelle B1 setzen (rechts von A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


