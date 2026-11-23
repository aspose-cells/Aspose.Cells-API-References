---
title: "PivotTable.ErrorString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide.

```csharp
public string ErrorString { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Définir la propriété ErrorString
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Calculer les données et actualiser le tableau croisé dynamique
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Enregistrez le classeur
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


