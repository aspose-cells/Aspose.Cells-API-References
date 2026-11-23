---
title: "Énumération TextCrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.TextCrossType. Enumère le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule"
type: docs
url: /fr/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Énumère le type d'affichage du texte lorsque la largeur du texte dépasse celle de la cellule.

```csharp
public enum TextCrossType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `1` | Afficher le texte comme dans Microsoft Excel. |
| CrossKeep | `2` | Afficher tout le texte en traversant d'autres cellules et conserver le texte des cellules traversées. |
| CrossOverride | `3` | Afficher tout le texte en traversant d'autres cellules et remplacer le texte des cellules traversées. |
| StrictInCell | `4` | Afficher uniquement le texte à l'intérieur de la largeur de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir un texte d'exemple dans une cellule qui pourrait déborder
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Créer des options d'image ou d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Démontrer différents paramètres TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


