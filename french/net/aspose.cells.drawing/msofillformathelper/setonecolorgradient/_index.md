---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode MsoFillFormatHelper. Définit le remplissage spécifié à un dégradé d’une seule couleur"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Définit le remplissage spécifié comme un dégradé d'une seule couleur.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Une couleur de dégradé. |
| degré | Double | Le degré du dégradé. Peut être une valeur de 0.0 (sombre) à 1.0 (clair). |
| style | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Placez une étiquette simple dans la feuille pour le contexte
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Créez une instance de MsoFillFormatHelper en utilisant la réflexion (pas de constructeur public)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Paramètres du dégradé
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Appliquez le dégradé d’une couleur
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Optionnel : montrer que les propriétés peuvent être lues après l’appel
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Enregistrez le classeur (aucun changement visuel ne sera observé car le helper n’est pas attaché à une forme)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


