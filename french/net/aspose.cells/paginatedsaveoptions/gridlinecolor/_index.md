---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Obtient ou définit la couleur des lignes de grille"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Obtient ou définit la couleur des lignes de grille.

```csharp
public Color GridlineColor { get; set; }
```

### Remarques

Il ignorera les paramètres de couleur des lignes de grille dans le fichier source.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Créez les options d'enregistrement PDF
                PdfSaveOptions options = new PdfSaveOptions();

                // Affichez la valeur par défaut de GridlineColor
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Définissez une nouvelle couleur de ligne de grille
                options.GridlineColor = Color.Red;

                // Affichez la valeur mise à jour de GridlineColor
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Enregistrez le classeur avec le paramètre de couleur des lignes de grille
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


