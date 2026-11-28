---
title: "SmartTag.SetLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTag yöntemi. Akıllı etiketin adını ve ad alanı URI'sini değiştirir."
type: docs
url: /tr/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Akıllı etiketin adını ve ad alanı URI'sını değiştir.

```csharp
public void SetLink(string uri, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uri | String | Akıllı etiketin ad alanı URI'si. |
| name | String | Akıllı etiketin adı. |

### Örnekler

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

### Ayrıca Bakınız

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


