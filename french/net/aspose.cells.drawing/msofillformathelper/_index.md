---
title: "Classe MsoFillFormatHelper"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.MsoFillFormatHelper. Représente le format de remplissage pour une forme"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Représente le format de remplissage d'une forme.

```csharp
public class MsoFillFormatHelper
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Obtient et définit la couleur d'arrière-plan du fichier. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Obtient et définit la couleur de premier plan du remplissage. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Obtient et définit les données de remplissage Texture et Image. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indique s'il y a un remplissage. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Obtient le type de remplissage de texture. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé d'une seule couleur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // Créez une instance de MsoFillFormatHelper en utilisant la réflexion
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Définir les propriétés de base
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // Afficher les valeurs des propriétés
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // Enregistrez le classeur
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


