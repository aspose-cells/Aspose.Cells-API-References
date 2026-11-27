---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption-metoden. Hämtar antalet områden som påverkas av denna inställning"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Hämtar antalet områden som påverkats av denna inställning.

```csharp
public int GetCountOfRange()
```

### Returvärde

antalet områden som påverkas av denna inställning.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hämta samling av felkontrollalternativ
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Lägg till första felkontrollalternativet
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Lägg till andra felkontrollalternativet
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Demonstrera GetCountOfRange-metoden
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Spara arbetsboken
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


