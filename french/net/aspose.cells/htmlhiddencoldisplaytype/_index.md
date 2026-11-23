---
title: "Enum HtmlHiddenColDisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.HtmlHiddenColDisplayType enum. Représente deux types d'affichage des colonnes cachées en HTML"
type: docs
url: /fr/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Représente deux types d'affichage des colonnes masquées en HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Hidden | `0` | Masquez les colonnes cachées dans la page HTML. |
| Remove | `1` | Supprimez les colonnes cachées dans la page HTML. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Masquez la deuxième colonne
            worksheet.Cells.HideColumn(1);

            // Créez HtmlSaveOptions et définissez le HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Enregistrer le classeur au format HTML
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


