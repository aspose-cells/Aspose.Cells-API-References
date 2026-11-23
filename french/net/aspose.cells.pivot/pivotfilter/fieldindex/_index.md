---
title: "PivotFilter.FieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient l'index du champ source auquel ce filtre pivot est appliqué"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Obtient l'index du champ source auquel ce filtre pivot est appliqué.

```csharp
public int FieldIndex { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un filtre
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField pivotField = pivotTable.PageFields[0];
            
            // Créer une collection de filtres pivot et ajouter un filtre
            PivotFilterCollection filters = pivotTable.PivotFilters;
            int filterIndex = filters.Add(0, PivotFilterType.Count);
            PivotFilter filter = filters[filterIndex];
            
            // Démontrer la propriété FieldIndex
            Console.WriteLine("Field Index: " + filter.FieldIndex);

            // Enregistrez le classeur
            workbook.Save("PivotFilterFieldIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


