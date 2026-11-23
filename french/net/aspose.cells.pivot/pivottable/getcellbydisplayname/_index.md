---
title: "PivotTable.GetCellByDisplayName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Obtient l'objet Cell par le nom d'affichage du PivotField"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Obtient l'objet [`Cell`](../../../aspose.cells/cell/) par le nom d'affichage du PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| displayName | String | le DisplayName du PivotField |

### Valeur de retour

l'objet Cell

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
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

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtenir le nom d'affichage du champ de données
            string displayName = pivotTable.DataFields[0].DisplayName;

            // Utiliser la méthode GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Afficher les résultats
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Enregistrez le classeur
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


