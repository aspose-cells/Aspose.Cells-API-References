---
title: "PivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte de l’en-tête du champ de la zone de valeurs dans le PivotTable"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/
---
## PivotGlobalizationSettings.GetTextOfDataFieldHeader method

Obtient le texte de l'en-tête du champ de la zone de valeurs dans le tableau croisé dynamique.

```csharp
public virtual string GetTextOfDataFieldHeader()
```

### Valeur de retour

Le texte du nom de l'en-tête du champ de données

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créez les paramètres de globalisation et démontrez la méthode GetTextOfDataFieldHeader
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Data Field Header Text: " + globalizationSettings.GetTextOfDataFieldHeader());

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


