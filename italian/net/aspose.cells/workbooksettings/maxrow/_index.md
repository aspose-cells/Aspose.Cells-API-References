---
title: "WorkbookSettings.MaxRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Restituisce l'indice massimo della riga con base zero"
type: docs
url: /it/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Ottiene l'indice massimo della riga, a base zero.

```csharp
public int MaxRow { get; }
```

### Osservazioni

Restituisce 65535 se il formato file è Excel97-2003;

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dimostrare la proprietà MaxRow
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Provare ad accedere a una cella oltre MaxRow (dovrebbe generare un'eccezione)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Creare un'area di celle usando MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


