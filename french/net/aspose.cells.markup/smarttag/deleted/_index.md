---
title: "SmartTag.Deleted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTag. Indique si le smart tag est supprimé"
type: docs
url: /fr/net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Indique si le smart tag est supprimé.

```csharp
public bool Deleted { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyDeletedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            Console.WriteLine("Initial Deleted value: " + smartTag.Deleted);

            // Définir la propriété Deleted sur true
            smartTag.Deleted = true;
            Console.WriteLine("After setting Deleted: " + smartTag.Deleted);

            // Enregistrez le classeur
            workbook.Save("SmartTagDeletedDemo.xlsx");

        }
    }
}
```

### Voir aussi

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


