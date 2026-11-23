---
title: "PivotTable.EnableDataValueEditing"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Spécifie une valeur booléenne qui indique si l’utilisateur est autorisé à modifier les cellules de la zone de données du pivottable. La valeur par défaut est false.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de EnableDataValueEditing
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Activer la modification des valeurs de données
            pivotTable.EnableDataValueEditing = true;

            // Calculer les données pour remplir le tableau croisé dynamique
            pivotTable.CalculateData();

            // Enregistrer le classeur avant la modification
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Nous pouvons maintenant modifier les valeurs de données directement dans le tableau croisé dynamique
            // À titre de démonstration, nous modifierons une cellule dans la zone de données
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Enregistrez le classeur après modification
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Désactiver la modification des valeurs de données
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


