---
title: "PivotPageFields.PivotPageFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur PivotPageFields. Représente les éléments du champ de page pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Représente les éléments de champ de page du tableau croisé dynamique.

```csharp
public PivotPageFields()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Créer des champs de page pivot en utilisant le constructeur
            PivotPageFields pageFields = new PivotPageFields();
            
            // Ajouter des champs de page
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Ajouter une identification
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Ajouter un tableau croisé dynamique avec les paramètres corrects
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Enregistrez le classeur
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


