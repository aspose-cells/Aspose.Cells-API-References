---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PptxSaveOptions. Représente le type de ligne dont la taille de police doit être ajustée si la hauteur de la ligne est petite"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Représente le type de ligne dont la taille de police doit être ajustée si la hauteur de la ligne est petite.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données et des lignes vides
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // Créer des options d’enregistrement PPTX
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // Enregistrer au format PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### Voir aussi

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


