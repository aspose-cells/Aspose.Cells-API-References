---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConditionalFormattingIcon. Obtient les données d'image avec le paramètre de cellule"
type: docs
url: /fr/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Obtient les données d'image avec le paramètre de la cellule.

```csharp
public byte[] GetImageData(Cell cell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellule | Cellule | Le paramètre de cellule. |

### Valeur de retour

Renvoie les données d'image de l'icône.

### Exemples

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


