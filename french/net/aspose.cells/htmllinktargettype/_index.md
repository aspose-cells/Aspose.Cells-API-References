---
title: "Enum HtmlLinkTargetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.HtmlLinkTargetType. Représente le type d'attribut target dans la balise HTML"
type: docs
url: /fr/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Représente le type d'attribut cible dans la balise HTML.

```csharp
public enum HtmlLinkTargetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Blank | `0` | Ouvre le document lié dans une nouvelle fenêtre ou un nouvel onglet |
| Parent | `1` | Ouvre le document lié dans le cadre parent |
| Self | `2` | Ouvre le document lié dans le même cadre que celui où il a été cliqué (c'est la valeur par défaut) |
| Top | `3` | Ouvre le document lié dans le corps complet de la fenêtre |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Créer HtmlSaveOptions et définir le LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Enregistrer le classeur au format HTML
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


