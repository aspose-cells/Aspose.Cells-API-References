---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SvgImageOptions. Obtient ou définit le type de police intégré dans le SVG"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Obtient ou définit le type de police intégré dans le SVG.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Remarques

La valeur par défaut est None, ce qui indique qu'aucune police ne sera intégrée dans le SVG.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données avec un formatage personnalisé pour démontrer l'intégration de police
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Créer des options de rendu SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Afficher le type de police intégré initial
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Rendre la feuille de calcul en SVG sans intégration de police
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Modifier le type de police intégré en WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Rendre la feuille de calcul en SVG avec intégration de police WOFF
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### Voir aussi

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


