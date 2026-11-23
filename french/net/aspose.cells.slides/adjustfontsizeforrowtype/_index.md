---
title: "Enum AdjustFontSizeForRowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Représente le type de lignes qui doit être ajusté"
type: docs
url: /fr/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Représente le type de lignes qui doivent être ajustées.

```csharp
public enum AdjustFontSizeForRowType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas d'ajustement. |
| EmptyRows | `1` | Si la ligne est vide, modifier la taille de la police pour correspondre à la hauteur de la ligne. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Créer une instance de PptxSaveOptions avec le paramètre AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Enregistrer le classeur au format PPTX
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


