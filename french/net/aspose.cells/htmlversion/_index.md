---
title: "Énumération HtmlVersion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.HtmlVersion. Indique la version de HTML utilisée lors de l'enregistrement aux formats HTML."
type: docs
url: /fr/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Indique la version de HTML utilisée lors de l'enregistrement aux formats HTML.

```csharp
public enum HtmlVersion
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Enregistrez le document conformément à l'exportation HTML de MS Excel. |
| XHtml | `1` | Enregistre le document conformément à la norme XHTML 1.0 Transitional. |
| Html5 | `2` | Enregistre le document conformément à la norme HTML 5. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Définir la version HTML sur HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Enregistrez le classeur avec la version HTML5
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Modifier la version HTML en XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Enregistrez le classeur avec la version XHTML
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Définir la version HTML sur Par défaut (compatible MS Excel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Enregistrez le classeur avec la version Par défaut
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


