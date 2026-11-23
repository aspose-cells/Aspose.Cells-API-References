---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s'il faut utiliser une unité évolutive pour décrire la largeur de l'image lorsqu'une unité évolutive est utilisée pour décrire la largeur de la colonne. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Indique s’il faut utiliser une unité évolutive pour décrire la largeur de l’image lorsqu’on utilise une unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true.

```csharp
public bool ImageScalable { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec une image
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image d'exemple à la feuille de calcul
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // Définir les options d'enregistrement HTML avec la propriété ImageScalable
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Enregistrez le classeur au format HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


