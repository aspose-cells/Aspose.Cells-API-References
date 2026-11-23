---
title: "FontConfigs.IsFontAvailable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Indique si la police est disponible"
type: docs
url: /fr/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Indique si la police est disponible.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | String | nom de police |

### Valeur de retour

true si la police est disponible, sinon false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tester les noms de police pour vérifier la disponibilité
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Appeler la méthode IsFontAvailable avec le nom de la police
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Afficher le résultat
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Écrire le résultat dans la feuille de calcul
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


