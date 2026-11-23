---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormatHelper. Indique s’il y a un remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indique s'il y a un remplissage.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une étiquette pour rendre l'exemple significatif
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Créer une instance de MsoFillFormatHelper en utilisant la réflexion (pas de constructeur public)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Affichez la valeur par défaut de IsVisible
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Définissez IsVisible sur true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Définissez IsVisible sur false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Lisez la valeur actuelle de IsVisible
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


