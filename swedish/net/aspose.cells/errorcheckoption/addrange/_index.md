---
title: "ErrorCheckOption.AddRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption-metod. Lägger till ett påverkad område med denna inställning"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Lägger till ett påverkad område med denna inställning.

```csharp
public int AddRange(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | området som ska läggas till. |

### Returvärde

indexen för det tillagda området i områdeslistan för denna inställning.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Lägg till områden med CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Spara arbetsboken
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


