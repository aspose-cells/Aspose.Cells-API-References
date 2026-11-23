---
title: "HtmlSaveOptions.DisableCss"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si seules des styles en ligne sont appliqués sans dépendre du CSS. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Indique si seuls les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false.

```csharp
public bool DisableCss { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple et le formatage
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Créer une instance de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Afficher la valeur actuelle de DisableCss
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Définir DisableCss sur true (en utilisant des styles en ligne au lieu du CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Définir DisableCss sur false (en utilisant des styles CSS)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Comparer les fichiers de sortie pour voir la différence d'approche de style
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


