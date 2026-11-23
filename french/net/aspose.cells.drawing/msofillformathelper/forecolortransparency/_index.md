---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormatHelper. Retourne ou définit le degré de couleur de premier plan du remplissage spécifié sous forme d’une valeur de 0,0 opaque à 1,0 transparent"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Renvoie ou définit le degré de couleur de premier plan du remplissage spécifié comme une valeur de 0.0 (opaque) à 1.0 (transparent).

```csharp
public double ForeColorTransparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une étiquette pour rendre l'exemple significatif
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Créer une instance de MsoFillFormatHelper en utilisant la réflexion (pas de constructeur public)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Afficher la valeur par défaut de ForeColorTransparency
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Définir un nouveau ForeColor et ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Afficher les valeurs mises à jour
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Démontrer la lecture de la valeur de transparence
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


