---
title: "PivotFieldSortSetting.SortType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldSortSetting. Représente l’ordre de tri"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Représente le [`SortOrder`](../../../aspose.cells/sortorder/).

```csharp
public SortOrder SortType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertySortTypeDemo
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
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Trier le champ de ligne par ordre croissant
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
            
            // Démontrer la propriété SortType
            Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Modifier l’ordre de tri et démontrer à nouveau
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
            Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


