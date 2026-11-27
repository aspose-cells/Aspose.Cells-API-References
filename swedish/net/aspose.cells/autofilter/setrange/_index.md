---
title: "AutoFilter.SetRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Anger det område som den angivna AutoFilter gäller för"
type: docs
url: /sv/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Ställer in intervallet som den angivna AutoFiltern gäller för.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| startColumn | Int32 | Startkolumnindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Ange autofilterområde (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Applicera filter
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Uppdatera filter
            sheet.AutoFilter.Refresh();

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


