---
title: "Classe CustomRenderSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.CustomRenderSettings. Représente les paramètres personnalisés pendant le rendu"
type: docs
url: /fr/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Représente les paramètres personnalisés pendant le rendu.

```csharp
public class CustomRenderSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Constructeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Spécifie la largeur de la bordure de la cellule selon le type de bordure. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Créez une instance de CustomRenderSettings en utilisant le constructeur par défaut
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Démontrez la méthode GetCellBorderWidth avec différents types de bordure
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Affichez les résultats
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Enregistrez le classeur
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


