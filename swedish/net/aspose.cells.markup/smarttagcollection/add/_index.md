---
title: "SmartTagCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagCollection-metod. Lägger till en smart tag"
type: docs
url: /sv/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Lägger till en smart tagg.

```csharp
public int Add(string uri, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uri | String | Anger namnrymdens URI för smart tag. |
| namn | String | Anger namnet på smart tag. |

### Returvärde

Indexet för smart tag i listan.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


