---
title: "Worksheet.SmartTagSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının tüm SmartTagCollection nesnelerini alır"
type: docs
url: /tr/net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Çalışma sayfasının tüm [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) nesnelerini alır.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


