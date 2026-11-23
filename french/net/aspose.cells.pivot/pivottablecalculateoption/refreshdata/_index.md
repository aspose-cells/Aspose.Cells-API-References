---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTableCalculateOption. Indique si la source de données du tableau croisé dynamique est rafraîchie"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indique si la source de données de rafraîchissement du tableau croisé dynamique.

```csharp
public bool RefreshData { get; set; }
```

### Remarques

Si c'est vrai, rafraîchir le cache du tableau croisé dynamique à partir de la source de données, puis calculer tous les tableaux croisés dynamiques basés sur le même cache.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Configurer des données d'exemple pour le tableau croisé dynamique
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Modifiez les données source
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Calculer le tableau croisé dynamique avec l'option RefreshData
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Afficher la valeur mise à jour du tableau croisé dynamique
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Voir aussi

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


