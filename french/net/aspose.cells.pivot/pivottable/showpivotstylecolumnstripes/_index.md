---
title: "PivotTable.ShowPivotStyleColumnStripes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si le format de bandes est appliqué pour la colonne"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/
---
## PivotTable.ShowPivotStyleColumnStripes property

Indique si le formatage en bandes est appliqué pour la colonne.

```csharp
public bool ShowPivotStyleColumnStripes { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnStripesDemo
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
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 12;
            
            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
            
            // Activer les bandes de colonne
            pivotTable.ShowPivotStyleColumnStripes = true;
            
            // Enregistrez le classeur
            workbook.Save("PivotTableColumnStripesDemo.xlsx");
            
            Console.WriteLine("Pivot table with column stripes created successfully.");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


