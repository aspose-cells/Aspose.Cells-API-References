---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte localisé de All Periods"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

Obtient le texte localisé de "All Periods".

```csharp
public virtual string GetTextOfAllPeriods()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOfAllPeriodsDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données d'exemple pour créer le contexte du tableau croisé dynamique
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // Créer un tableau croisé dynamique
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Créer une instance de PivotGlobalizationSettings
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // Démontrer la méthode GetTextOfAllPeriods
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // Afficher les libellés de périodes temporelles associés pour le contexte
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // Enregistrez le classeur
                workbook.Save("GetTextOfAllPeriodsDemo.xlsx");
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

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


