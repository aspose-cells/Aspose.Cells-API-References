---
title: "Workbook.RemoveUnusedStyles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ta bort alla oanvända stilar"
type: docs
url: /sv/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Ta bort alla oanvända format.

```csharp
public void RemoveUnusedStyles()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata med stilar
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Applicera olika stilar på celler
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Ta bort några celler för att lämna oanvända stilar
            sheet.Cells.DeleteRows(5, 5);
            
            // Spara innan oanvända stilar tas bort
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Ta bort oanvända stilar
            wb.RemoveUnusedStyles();
            
            // Spara efter att oanvända stilar har tagits bort
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


