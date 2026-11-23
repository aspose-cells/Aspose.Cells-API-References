---
title: "PivotTable.IsGridDropZones"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si le rapport PivotTable affiche la mise en page classique du tableau croisé dynamique. active le glisser-déposer des champs dans la grille"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Indique si le rapport du tableau croisé dynamique affiche la disposition classique du tableau croisé dynamique. (permet de faire glisser les champs dans la grille)

```csharp
public bool IsGridDropZones { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsGridDropZonesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
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
            worksheet.Cells["B4"].Value = 300;

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Définir la propriété IsGridDropZones
            pivotTable.IsGridDropZones = true;
            Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);

            // Enregistrez le classeur
            workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


