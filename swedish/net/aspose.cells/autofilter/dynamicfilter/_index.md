---
title: "AutoFilter.DynamicFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett dynamiskt filter"
type: docs
url: /sv/net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

Lägger till ett dynamiskt filter.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| dynamicFilterType | DynamicFilterType | Dynamisk filtertyp. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            // Tillämpa autofilter med korrekt metodsignatur
            worksheet.AutoFilter.Range = "A1:A6";

            // Tillämpa dynamiskt filter för marsdatum
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


