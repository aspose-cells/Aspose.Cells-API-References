---
title: "SmartTag.SetLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SmartTag. Modifie le nom et l'URI d'espace de noms du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Modifie le nom et l'URI de l'espace de noms du smart tag.

```csharp
public void SetLink(string uri, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | String | L'URI d'espace de noms du smart tag. |
| name | String | Le nom du smart tag. |

### Exemples

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

### Voir aussi

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


