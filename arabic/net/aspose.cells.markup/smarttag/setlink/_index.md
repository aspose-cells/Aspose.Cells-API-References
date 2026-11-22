---
title: "SmartTag.SetLink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SmartTag. تغيير الاسم ومسار URI للمساحة الاسمية للعلامة الذكية"
type: docs
url: /ar/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

غيّر الاسم وURI مساحة الاسم للعلامة الذكية.

```csharp
public void SetLink(string uri, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| uri | String | مسار URI للمساحة الاسمية للعلامة الذكية. |
| name | String | اسم العلامة الذكية. |

### أمثلة

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

### انظر أيضًا

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


