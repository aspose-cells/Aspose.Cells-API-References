---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Optimise la sortie du html en utilisant des propriétés CSS personnalisées. Par exemple, dans le cas où il existe plusieurs occurrences d'une même image base64 avec une propriété personnalisée, les données de l'image n'ont besoin d'être enregistrées qu'une seule fois, ce qui améliore les performances du html résultant. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Optimisez la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où il y a plusieurs occurrences d'une même image base64, avec une propriété personnalisée les données de l'image ne doivent être enregistrées qu'une fois, ce qui améliore les performances du html résultant. La valeur par défaut est false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec mise en forme
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Ajouter une image qui sera répétée dans plusieurs cellules
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Copier l'image vers un autre emplacement
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Créer une instance de HtmlSaveOptions
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Afficher la valeur actuelle
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Définir sur true pour optimiser la sortie CSS
            htmlOptions.EnableCssCustomProperties = true;

            // Enregistrer avec optimisation CSS
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Définir sur false pour la comparaison
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


