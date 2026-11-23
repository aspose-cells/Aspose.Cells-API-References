---
title: "PivotGlobalizationSettings.GetTextOfProtection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le nom de protection dans le PivotTable"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/
---
## PivotGlobalizationSettings.GetTextOfProtection method

Obtient le nom de protection dans le tableau croisé dynamique.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetTextOfProtection()
```

### Valeur de retour

Le nom de protection du tableau croisé dynamique

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetTextOfProtectedName(string). Cette propriété sera supprimée 12 mois plus tard à partir de mars 2023. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectionDemo
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

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créez les paramètres de mondialisation et démontrez GetTextOfProtection
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Protection Text: " + globalizationSettings.GetTextOfProtection());

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


