---
title: "SmartTag.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTag. Obtient le nom du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Obtient le nom du smart tag.

```csharp
public string Name { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyNameDemo
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

            // Démontrer la propriété Name (opération en lecture seule)
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Enregistrez le classeur
            workbook.Save("SmartTagNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


