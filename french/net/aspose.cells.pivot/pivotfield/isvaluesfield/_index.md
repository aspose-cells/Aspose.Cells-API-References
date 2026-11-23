---
title: "PivotField.IsValuesField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si ce champ représente le champ de valeurs"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/isvaluesfield/
---
## PivotField.IsValuesField property

Indique si ce champ représente un champ de valeurs.

```csharp
public bool IsValuesField { get; }
```

### Remarques

Fonctionne uniquement lorsqu'il y a deux champs de données ou plus dans la vue du tableau croisé dynamique.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValuesFieldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";

            cells["A2"].Value = "Fruit";
            cells["B2"].Value = "Apple";
            cells["C2"].Value = 100;

            cells["A3"].Value = "Fruit";
            cells["B3"].Value = "Orange";
            cells["C3"].Value = 150;

            cells["A4"].Value = "Vegetable";
            cells["B4"].Value = "Carrot";
            cells["C4"].Value = 200;

            cells["A5"].Value = "Vegetable";
            cells["B5"].Value = "Potato";
            cells["C5"].Value = 250;

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Obtenir le champ de données (Ventes)
                PivotField dataField = pivotTable.DataFields[0];

                // Afficher la valeur de la propriété IsValuesField
                Console.WriteLine("IsValuesField value: " + dataField.IsValuesField);

                // Obtenir un champ de ligne (Catégorie) pour comparaison
                PivotField rowField = pivotTable.RowFields["Category"];
                Console.WriteLine("Row field IsValuesField value: " + rowField.IsValuesField);

                // Calculer les données et actualiser
                pivotTable.CalculateData();

                // Enregistrez le classeur
                workbook.Save("IsValuesFieldDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


