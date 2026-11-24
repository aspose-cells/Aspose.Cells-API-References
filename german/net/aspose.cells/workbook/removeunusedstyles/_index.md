---
title: "Workbook.RemoveUnusedStyles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Entfernt alle ungenutzten Stile"
type: docs
url: /de/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Entfernt alle ungenutzten Stile.

```csharp
public void RemoveUnusedStyles()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            
            // Füge einige Beispieldaten mit Stilen hinzu
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Wende verschiedene Stile auf Zellen an
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Entferne einige Zellen, um ungenutzte Stile zu hinterlassen
            sheet.Cells.DeleteRows(5, 5);
            
            // Speichern vor dem Entfernen ungenutzter Stile
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Ungenutzte Stile entfernen
            wb.RemoveUnusedStyles();
            
            // Speichern nach dem Entfernen ungenutzter Stile
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


