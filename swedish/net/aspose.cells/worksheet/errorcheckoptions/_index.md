---
title: "Worksheet.ErrorCheckOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar felkontrollinställning som tillämpas på vissa områden"
type: docs
url: /sv/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Hämtar felkontrollinställning som tillämpas på vissa områden.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aktivera felkontrollalternativ
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Hämta antalet områden för alternativet
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Spara arbetsboken
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


