---
title: "SmartTagCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagCollection-Methode. Fügt einen SmartTag hinzu"
type: docs
url: /de/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Fügt ein SmartTag hinzu.

```csharp
public int Add(string uri, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uri | String | Gibt die Namespace-URI des SmartTags an |
| Name | String | Gibt den Namen des SmartTags an. |

### Rückgabewert

Der Index des SmartTags in der Liste.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


