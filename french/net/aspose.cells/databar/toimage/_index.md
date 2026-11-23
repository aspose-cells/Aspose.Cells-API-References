---
title: "DataBar.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DataBar. Rendre la barre de données dans la cellule en tableau d'octets d'image"
type: docs
url: /fr/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Rendre le DataBar dans la cellule en tableau d'octets d'image.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellule | Cellule | Indiquer la barre de données dans quelle cellule doit être rendue |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contient certaines propriétés de l'image de sortie |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et un formatage conditionnel
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Ajouter une mise en forme conditionnelle de barre de données
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Obtenir la cellule avec le format conditionnel
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Convertir la barre de données en image
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Enregistrer l'image
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Pour la vérification d'image, vous devez ajouter le package System.Drawing.Common
                // et utiliser System.Drawing.Image si nécessaire
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


