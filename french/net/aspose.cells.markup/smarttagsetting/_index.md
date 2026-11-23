---
title: "Classe SmartTagSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Markup.SmartTagSetting. Représente tous les objets SmartTagCollection dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Représente tous les objets [`SmartTagCollection`](../smarttagcollection/) dans la feuille de calcul.

```csharp
public class SmartTagSetting : CollectionBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Obtient un objet [`SmartTagCollection`](../smarttagcollection/) par l'index. (3 indexeurs) |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Ajoute des smart tags à la cellule. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Ajoute un objet [`SmartTagCollection`](../smarttagcollection/) à une cellule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute un smart tag à une cellule spécifique
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Accéder à la SmartTagCollection pour la cellule
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Ajouter une smart tag à la collection
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Définir la capacité du paramètre de smart tag
            smartTagSetting.Capacity = 10;

            // Imprimer le nombre de smart tags
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Enregistrez le classeur
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


