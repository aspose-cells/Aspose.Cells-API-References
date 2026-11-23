---
title: "PivotField.ShowAllItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique s'il faut afficher tous les éléments dans la vue du tableau croisé même s'ils ne contiennent pas de données de synthèse. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. La valeur par défaut est false.

```csharp
public bool ShowAllItems { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Définir la propriété ShowAllItems pour le champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Calculez les données et enregistrez
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


