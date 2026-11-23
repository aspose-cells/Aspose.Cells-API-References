---
title: "PivotGlobalizationSettings.GetTextOfSeconds"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local des secondes"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/
---
## PivotGlobalizationSettings.GetTextOfSeconds method

Obtient le texte local de "Seconds"

```csharp
public virtual string GetTextOfSeconds()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajoutez le champ de date à la zone de lignes
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Créer des paramètres de mondialisation
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Démontrer la méthode GetTextOfSeconds
            Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());

            // Enregistrez le classeur
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


