---
title: "Style.GetTwoColorGradientSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Obtient le paramètre de dégradé à deux couleurs"
type: docs
url: /fr/net/aspose.cells/style/gettwocolorgradientsetting/
---
## Style.GetTwoColorGradientSetting method

Obtenir le paramètre de dégradé bicolore.

```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style et définir un dégradé à deux couleurs
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            style.IsGradient = true;

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            cell.SetStyle(style);

            try
            {
                // Appeler la méthode GetTwoColorGradientSetting
                TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();

                // Afficher les paramètres du dégradé
                Console.WriteLine("Color1: " + gradientSetting.Color1);
                Console.WriteLine("Color2: " + gradientSetting.Color2);
                Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
                Console.WriteLine("Variant: " + gradientSetting.Variant);

                // Modifier les paramètres du dégradé
                gradientSetting.Color1 = Color.Green;
                gradientSetting.GradientStyleType = GradientStyleType.Vertical;
                style.SetTwoColorGradient(gradientSetting.Color1, gradientSetting.Color2, 
                                        gradientSetting.GradientStyleType, gradientSetting.Variant);

                Console.WriteLine("Gradient settings modified successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradientSetting method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


