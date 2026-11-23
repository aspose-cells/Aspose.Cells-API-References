---
title: "SmartTagPropertyCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SmartTagPropertyCollection. Ajoute une propriété de balise intelligente de cellules"
type: docs
url: /fr/net/aspose.cells.markup/smarttagpropertycollection/add/
---
## SmartTagPropertyCollection.Add method

Ajoute une propriété du smart tag de la cellule.

```csharp
public int Add(string name, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété |
| valeur | String | La valeur de la propriété. |

### Valeur de retour

retourner [`SmartTagProperty`](../../smarttagproperty/)

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Voir aussi

* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


