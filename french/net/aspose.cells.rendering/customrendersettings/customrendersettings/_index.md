---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur CustomRenderSettings. Ctor"
type: docs
url: /fr/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Constructeur.

```csharp
public CustomRenderSettings()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Créer une instance de CustomRenderSettings à l'aide du constructeur
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Afficher la confirmation de l'appel réussi du constructeur
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Démontrer que l'instance est fonctionnelle en appelant une méthode
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Enregistrez le classeur
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


