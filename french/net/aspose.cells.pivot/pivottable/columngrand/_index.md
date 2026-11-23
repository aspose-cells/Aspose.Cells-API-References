---
title: "PivotTable.ColumnGrand"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si le rapport PivotTable affiche les totaux généraux pour les colonnes"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/columngrand/
---
## PivotTable.ColumnGrand property

Indique si le rapport PivotTable affiche les totaux généraux pour les colonnes.

```csharp
[Obsolete("Use PivotTable.ShowColumnGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ColumnGrand { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.ShowColumnGrandTotals. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyColumnGrandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Afficher la valeur actuelle de ColumnGrand
            Console.WriteLine("Current ColumnGrand value: " + pivotTable.ColumnGrand);

            // Modifier la propriété ColumnGrand
            pivotTable.ColumnGrand = false;

            // Calculer les données pour voir l'effet
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableColumnGrandDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


