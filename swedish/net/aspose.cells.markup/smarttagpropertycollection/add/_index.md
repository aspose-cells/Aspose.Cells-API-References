---
title: "SmartTagPropertyCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagPropertyCollection‑metod. Lägger till en egenskap för cellers smarta tagg"
type: docs
url: /sv/net/aspose.cells.markup/smarttagpropertycollection/add/
---
## SmartTagPropertyCollection.Add method

Lägger till en egenskap för cellens smarta tagg.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen |
| värde | String | Värdet på egenskapen. |

### Returvärde

returnera [`SmartTagProperty`](../../smarttagproperty/)

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Se även

* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


