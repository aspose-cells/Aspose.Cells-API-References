---
title: "Worksheet.SmartTagSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает все объекты SmartTagCollection листа"
type: docs
url: /ru/net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Получает все объекты [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) листа.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySmartTagSettingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());

            workbook.Save("SmartTagSettingDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


