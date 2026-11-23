---
title: "WorkbookSettings.HidePivotFieldList"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit si la liste des champs du PivotTable est masquée"
type: docs
url: /fr/net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Obtient et définit si la liste des champs du PivotTable est masquée.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyHidePivotFieldListDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(150);

            // Créer un tableau croisé dynamique
            int index = workbook.Worksheets.Add(SheetType.Worksheet);
            Worksheet pivotSheet = workbook.Worksheets[index];
            pivotSheet.Name = "PivotTable";
            
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accéder aux paramètres du classeur et définir la propriété HidePivotFieldList
            WorkbookSettings settings = workbook.Settings;
            settings.HidePivotFieldList = true; // Hide the pivot field list

            // Enregistrez le classeur
            workbook.Save("HidePivotFieldListDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


