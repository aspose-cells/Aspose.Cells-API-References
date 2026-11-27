---
title: "AutoFilter.Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Filtrerar en lista med angivna kriterier"
type: docs
url: /sv/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filtrerar en lista med specificerade kriterier.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| kriterier | String | Det angivna kriteriet (en sträng; till exempel, "101"). |

### Anmärkningar

Aspose.Cells kommer att ta bort alla andra filterinställningar på detta fält som i MS Excel 97-2003.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Applicera autofilter med korrekta SetRange-parametrar
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Spara resultatet
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


