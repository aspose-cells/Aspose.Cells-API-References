---
title: "PivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte de l'étiquette Multiple Items dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/
---
## PivotGlobalizationSettings.GetTextOfMultipleItems method

Obtient le texte de l'étiquette "(Multiple Items)" dans le tableau croisé dynamique.

```csharp
public virtual string GetTextOfMultipleItems()
```

### Valeur de retour

Le texte de l’étiquette "(Multiple Items)"

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créez et utilisez les paramètres de globalisation
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Démontrer GetTextOfMultipleItems et d'autres méthodes clés
            Console.WriteLine("Multiple Items Text: " + settings.GetTextOfMultipleItems());
            Console.WriteLine("Total Text: " + settings.GetTextOfTotal());
            Console.WriteLine("Grand Total Text: " + settings.GetTextOfGrandTotal());

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


