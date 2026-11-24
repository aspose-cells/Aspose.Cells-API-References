---
title: "Worksheet.SmartTagSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt alle SmartTagCollection-Objekte des Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Gibt alle [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) Objekte des Arbeitsblatts zurück.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Beispiele

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

### Siehe auch

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


