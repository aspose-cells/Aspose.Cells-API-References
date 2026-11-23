---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit le type de police intégrée dans le fichier html. La valeur par défaut est None, ce qui indique qu'aucune police ne sera intégrée dans le html."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Obtient ou définit le type d'intégration du fichier de police dans le fichier html. La valeur par défaut est None, ce qui indique qu'aucune police ne sera intégrée dans le html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Créer des options d'enregistrement HTML
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Afficher la valeur par défaut de EmbeddedFontType
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Définir EmbeddedFontType sur Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Enregistrer le classeur avec l'intégration de police WOFF
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Réinitialiser à None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Enregistrer le classeur sans intégration de police
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


