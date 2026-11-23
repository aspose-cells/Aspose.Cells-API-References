---
title: "Enumération HtmlHiddenRowDisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enumération Aspose.Cells.HtmlHiddenRowDisplayType. Représente deux types d'affichage des lignes masquées en HTML"
type: docs
url: /fr/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Représente deux types d'affichage des lignes masquées en HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Hidden | `0` | Masquer les lignes cachées dans la page HTML. |
| Remove | `1` | Supprimer les lignes cachées dans la page HTML. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Masquer la deuxième ligne
            worksheet.Cells.HideRow(1);

            // Créer HtmlSaveOptions et définir le HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Enregistrer le classeur au format HTML
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


