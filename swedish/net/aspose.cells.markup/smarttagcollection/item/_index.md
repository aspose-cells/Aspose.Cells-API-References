---
title: "SmartTagCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagCollection-egenskap. Hämtar ett SmartTag-objekt på det specifika indexet"
type: docs
url: /sv/net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Hämtar ett [`SmartTag`](../../smarttag/) objekt på det specifika indexet

```csharp
public SmartTag this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

returnerar ett [`SmartTag`](../../smarttag/) objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Demonstrera användning av Item-egenskapen
            SmartTagProperty authorProperty = properties["Author"];
            Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Se även

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


