---
title: "SmartTag.Uri"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTag. Obtient l'URI d'espace de noms du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Obtient l'URI de l'espace de noms du smart tag.

```csharp
public string Uri { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyUriDemo
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

            // Affiche la valeur de la propriété Uri (opération en lecture seule)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Démontrez d'autres propriétés
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Enregistrez le classeur
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


