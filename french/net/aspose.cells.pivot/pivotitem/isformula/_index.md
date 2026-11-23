---
title: "PivotItem.IsFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItem. Indique si cet élément pivot est un élément de formule calculée"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Indique si cet élément pivot est un élément de formule calculée.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotItem.IsCalculatedItem. Cette propriété sera supprimée 12 mois plus tard, à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenir le premier élément pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Afficher la valeur actuelle de IsFormula (propriété obsolète)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Définir une nouvelle valeur pour IsFormula (propriété obsolète)
            pivotItem.IsFormula = true;

            // Démontrer l'effet - cela marquerait l'élément pivot comme un élément de formule
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Remarque : Dans une utilisation réelle, vous devez utiliser IsCalculatedItem à la place car IsFormula est obsolète
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Enregistrer le résultat
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


