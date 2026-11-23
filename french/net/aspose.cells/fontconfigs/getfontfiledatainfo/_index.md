---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Obtenir les informations de données du fichier de police"
type: docs
url: /fr/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Obtenir les informations de données du fichier de police.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | String | nom de police |
| isBold | Boolean | le style de police est en gras ou non |
| isItalic | Boolean | le style de police est en italique ou non |
| isExactStyle | Boolean | si l'on doit correspondre exactement au style gras/italique donné |

### Valeur de retour

Informations de données du fichier de police.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Appeler GetFontFileDataInfo avec des paramètres spécifiques (modifié en appel statique)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Afficher les informations sur les données du fichier de police
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Démontrer l'effet sur un classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Définir le style avec la police que nous avons vérifiée
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Appliquer le style à une cellule
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Enregistrez le classeur
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


