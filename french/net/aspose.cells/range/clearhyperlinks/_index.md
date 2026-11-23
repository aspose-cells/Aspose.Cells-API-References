---
title: "Range.ClearHyperlinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Supprime uniquement les hyperliens"
type: docs
url: /fr/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Supprime uniquement les hyperliens.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clearFormat | Boolean | Indique s'il faut supprimer le format des hyperliens. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage et ajouter quelques hyperliens à titre de démonstration
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Effacer les hyperliens avec préservation du format (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Ajouter à nouveau les hyperliens
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Effacer les hyperliens sans préservation du format (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Enregistrez le classeur
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


