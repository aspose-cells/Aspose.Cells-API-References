---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit le mode de mise en page lors de l'enregistrement en HTML. La valeur par défaut est Normal"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Obtient ou définit le mode de mise en page lors de l’enregistrement en HTML. La valeur par défaut est Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Créer une instance de HtmlSaveOptions
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Afficher la valeur actuelle de LayoutMode
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Définir LayoutMode sur Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Enregistrer le classeur avec le mode de mise en page Print
                workbook.Save("LayoutModePrint.html", options);

                // Définir LayoutMode sur Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Enregistrer le classeur avec le mode de mise en page Normal
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


