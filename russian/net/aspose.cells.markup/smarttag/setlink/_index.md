---
title: "SmartTag.SetLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SmartTag. Изменить имя и URI пространства имён смарт-тега"
type: docs
url: /ru/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Изменяет имя и URI пространства имён смарт‑тега.

```csharp
public void SetLink(string uri, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | String | URI пространства имён смарт-тега. |
| name | String | Имя смарт-тега. |

### Примеры

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

### См. также

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


