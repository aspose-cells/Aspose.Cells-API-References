---
title: "SmartTagCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SmartTagCollection. Ajoute un smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Ajoute une smart tag.

```csharp
public int Add(string uri, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uri | String | Spécifie l'URI d'espace de noms du smart tag |
| name | String | Spécifie le nom du smart tag. |

### Valeur de retour

L'index du smart tag dans la liste.

### Exemples

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

### Voir aussi

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


