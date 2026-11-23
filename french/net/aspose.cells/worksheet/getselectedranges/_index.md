---
title: "Worksheet.GetSelectedRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur"
type: docs
url: /fr/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Valeur de retour

Une ArrayList contenant les plages sélectionnées.

### Remarques

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode Worksheet.GetSelectedAreas(). Cette propriété sera supprimée 12 mois plus tard à compter de mars 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Remarque : GetSelectedRanges est marqué comme obsolète dans la réflexion
                // Ceci démontre l'appel de la méthode tel que demandé
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Afficher le nombre de plages sélectionnées
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Afficher chaque plage sélectionnée
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Enregistrez le classeur
                workbook.Save("GetSelectedRangesDemo.xlsx");
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


