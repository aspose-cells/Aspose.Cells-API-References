---
title: "SmartTagPropertyCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SmartTagPropertyCollection. تُضيف خاصية لعلامة ذكية للخلية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagpropertycollection/add/
---
## SmartTagPropertyCollection.Add method

يضيف خاصية لعلامة ذكية للخلية.

```csharp
public int Add(string name, string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية |
| القيمة | String | قيمة الخاصية. |

### قيمة الإرجاع

إرجاع [`SmartTagProperty`](../../smarttagproperty/)

### أمثلة

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

### انظر أيضًا

* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


