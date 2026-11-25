---
title: "Workbook.RemoveUnusedStyles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Rimuove tutti gli stili non utilizzati"
type: docs
url: /it/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Rimuove tutti gli stili inutilizzati.

```csharp
public void RemoveUnusedStyles()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio con gli stili
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Applica stili diversi alle celle
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Rimuovi alcune celle per lasciare stili non utilizzati
            sheet.Cells.DeleteRows(5, 5);
            
            // Salva prima di rimuovere gli stili non utilizzati
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Rimuovi gli stili inutilizzati
            wb.RemoveUnusedStyles();
            
            // Salva dopo aver rimosso gli stili inutilizzati
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


