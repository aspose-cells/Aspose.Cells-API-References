---
title: "Enum SaveElementType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Saving.SaveElementType. Représente le type d'éléments à enregistrer"
type: docs
url: /fr/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Représente le type d'éléments qui doivent être enregistrés.

```csharp
public enum SaveElementType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| All | `251658239` | Toutes les données. |
| Chart | `256` | Uniquement les graphiques. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple pour démontrer l'enregistrement
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Créer un graphique pour démontrer le type d'élément d'enregistrement du graphique
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Démontrer l'utilisation des valeurs de l'enum SaveElementType
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Enregistrer le classeur avec tous les éléments
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


