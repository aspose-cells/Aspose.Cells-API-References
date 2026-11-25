---
title: "WorkbookSettings.MaxColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene l'indice massimo della colonna basato su zero"
type: docs
url: /it/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Ottiene l'indice massimo della colonna, a base zero.

```csharp
public int MaxColumn { get; }
```

### Osservazioni

Restituisce 255 se il formato file è Excel97-2003;

### Esempi

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
            
            // Dimostra l'uso di MaxColumn provando ad accedere a una colonna oltre il limite
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

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


