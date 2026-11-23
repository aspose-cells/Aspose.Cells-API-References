---
title: "Classe SmartTag"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Markup.SmartTag. Représente un smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Représente une balise intelligente.

```csharp
public class SmartTag
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Indique si le smart tag est supprimé. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Obtient le nom du smart tag. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Obtient et définit les propriétés du smart tag. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Obtient l'URI de l'espace de noms du smart tag. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Modifie le nom et l'URI de l'espace de noms du smart tag. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassSmartTagDemo
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

            workbook.Save("SmartTagDemo.xlsx");
            Console.WriteLine("SmartTagDemo.xlsx created successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


