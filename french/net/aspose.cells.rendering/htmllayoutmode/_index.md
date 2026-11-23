---
title: "Énumération HtmlLayoutMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Rendering.HtmlLayoutMode. Représente le mode de mise en page pour le rendu HTML"
type: docs
url: /fr/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Représente le mode de mise en page pour le rendu HTML.

```csharp
public enum HtmlLayoutMode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Normal | `0` | Rend le contenu comme MS Excel. |
| Print | `1` | Rend le contenu en mode mise en page d'impression. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Créez HtmlSaveOptions et définissez le mode de mise en page sur Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Enregistrez le classeur avec le mode de mise en page normal
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Changez le mode de mise en page en Impression
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Enregistrez le classeur avec le mode de mise en page d'impression
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Afficher les valeurs d'énumération
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


