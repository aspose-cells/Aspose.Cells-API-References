---
title: "SmartTag.SetLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTag-Methode. Ändern Sie den Namen und die Namespace-URI des SmartTags"
type: docs
url: /de/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Ändere den Namen und den Namespace‑URI des Smart‑Tags.

```csharp
public void SetLink(string uri, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | String | Die Namespace-URI des SmartTags. |
| Name | String | Der Name des SmartTags. |

### Beispiele

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

### Siehe auch

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


