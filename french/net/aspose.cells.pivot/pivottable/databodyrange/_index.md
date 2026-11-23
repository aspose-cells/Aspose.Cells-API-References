---
title: "PivotTable.DataBodyRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Retourne un objet CellArea qui représente la plage contenant la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seule"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Retourne un objet [`CellArea`](../../../aspose.cells/cellarea/) qui représente la plage contenant la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seule.

```csharp
public CellArea DataBodyRange { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Ajouter un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Configurer le tableau croisé dynamique
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualiser les données du tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();

            // Démontrer l'utilisation de DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Enregistrez le classeur
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


