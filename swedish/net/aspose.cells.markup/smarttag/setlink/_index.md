---
title: "SmartTag.SetLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTag-metod. Ändra namnet och namnrymdens URI för smart tag"
type: docs
url: /sv/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Ändra namnet och namnrymdens URI för den smarta taggen.

```csharp
public void SetLink(string uri, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uri | String | Namnrymdens URI för smart tag. |
| namn | String | Namnet på smart tag. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagMethodSetLinkWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            workbook.Save("SmartTagSetLinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


