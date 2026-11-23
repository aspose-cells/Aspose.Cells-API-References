---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomRenderSettings. Spécifie la largeur de la bordure de cellule selon le type de bordure"
type: docs
url: /fr/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Spécifie la largeur de la bordure de la cellule selon le type de bordure.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | CellBorderType | type de bordure de cellule |

### Valeur de retour

largeur de la bordure de cellule

### Remarques

Toute valeur négative sera ignorée.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une instance de CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Appeler GetCellBorderWidth avec différents types de bordure
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Affichez les résultats
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Enregistrez le classeur
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


