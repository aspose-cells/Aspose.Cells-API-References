---
title: "Worksheet.SmartTagSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient tous les objets SmartTagCollection de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Obtient tous les objets [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) de la feuille de calcul.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Exemples

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

### Voir aussi

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


