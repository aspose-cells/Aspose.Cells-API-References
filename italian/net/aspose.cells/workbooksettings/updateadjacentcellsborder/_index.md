---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se aggiornare il bordo delle celle adiacenti"
type: docs
url: /it/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Indica se aggiornare il bordo delle celle adiacenti.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Osservazioni

Il valore predefinito è false. Per esempio: il bordo inferiore della cella A1 è aggiornato, il bordo superiore della cella A2 dovrebbe essere cambiato anch'esso.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Abilita l'aggiornamento dei bordi delle celle adiacenti
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta il valore e applica il bordo alla cella A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Imposta il valore nella cella adiacente B1 (a destra di A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


