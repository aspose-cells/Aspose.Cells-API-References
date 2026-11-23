---
title: "PivotGlobalizationSettings.GetTextOfRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local de Range"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrange/
---
## PivotGlobalizationSettings.GetTextOfRange method

Obtient le texte local de "Range"

```csharp
public virtual string GetTextOfRange()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer les paramètres de mondialisation et démontrer GetTextOfRange
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

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


