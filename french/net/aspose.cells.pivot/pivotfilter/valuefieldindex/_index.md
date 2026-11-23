---
title: "PivotFilter.ValueFieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient l'index du champ de valeur dans la région des valeurs"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

Obtient l'index du champ de valeur dans la région de valeur.

```csharp
public int ValueFieldIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValueFieldIndexDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
            
            // Ajouter un filtre de comptage au champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Obtenir le filtre et démontrer ValueFieldIndex
            PivotFilter filter = rowField.GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            
            // Enregistrez le classeur
            workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


