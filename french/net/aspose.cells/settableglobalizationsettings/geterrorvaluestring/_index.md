---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient la chaîne d’affichage pour la valeur d’erreur des cellules"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Obtient la chaîne d'affichage de la valeur d'erreur de la cellule

```csharp
public override string GetErrorValueString(string err)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| err | String | valeurs d'erreur telles que #VALUE!,#NAME? |

### Valeur de retour

Par défaut, renvoie la valeur d'erreur elle-même

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Créer une cellule avec une valeur d'erreur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Appeler GetErrorValueString avec la chaîne de valeur d'erreur
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Afficher le résultat
                Console.WriteLine("Error value string: " + errorString);

                // Afficher l'effet en définissant la valeur d'une autre cellule sur la chaîne renvoyée
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


