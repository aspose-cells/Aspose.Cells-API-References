---
title: "PivotTable.PivotTableStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient ou définit le nom du style du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/pivottablestylename/
---
## PivotTable.PivotTableStyleName property

Obtient ou définit le nom du style du tableau croisé dynamique.

```csharp
public string PivotTableStyleName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Data;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Appliquer un style de tableau croisé dynamique intégré
            pivotTable.PivotTableStyleName = "PivotStyleLight16";
            
            // Enregistrez le classeur
            workbook.Save("PivotTableStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


