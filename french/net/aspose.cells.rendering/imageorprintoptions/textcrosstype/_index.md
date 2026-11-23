---
title: "ImageOrPrintOptions.TextCrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir un texte long qui dépassera la largeur de la cellule
            worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
            worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;

            // Créer des options d'image ou d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Démontrer différents paramètres TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveAsImage(workbook, options, "TextCrossType_Default.png");

            options.TextCrossType = TextCrossType.CrossKeep;
            SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");

            options.TextCrossType = TextCrossType.CrossOverride;
            SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");

            options.TextCrossType = TextCrossType.StrictInCell;
            SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
        }

        private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Voir aussi

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


