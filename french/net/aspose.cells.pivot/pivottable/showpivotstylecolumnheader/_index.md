---
title: "PivotTable.ShowPivotStyleColumnHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si l’en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showpivotstylecolumnheader/
---
## PivotTable.ShowPivotStyleColumnHeader property

Indique si l'en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué.

```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnHeaderDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Définissez le style du tableau croisé dynamique
            pivotTable.ShowPivotStyleColumnHeader = true;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowPivotStyleColumnHeaderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


