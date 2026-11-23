---
title: "PivotField.SortSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient tous les paramètres du tri automatique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

Obtient tous les paramètres du tri automatique

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertySortSettingDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 75;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];

            // Démontrer la propriété SortSetting
            rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);

            // Modifier les paramètres de tri
            rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
            Console.WriteLine("\nAfter changing sort settings:");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Voir aussi

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


