---
title: "Enum PivotItemPositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotItemPositionType enum. Représente le type de position de l'élément de base du tableau croisé dynamique dans le champ de base lorsque le calcul ShowDataAs est utilisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Représente le type de position de l'élément de base du tableau croisé dynamique dans le champ de base lorsque le calcul ShowDataAs est utilisé.

```csharp
public enum PivotItemPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Previous | `0` | Représente l'élément pivot précédent dans le PivotField. |
| Next | `1` | Représente l'élément pivot suivant dans le PivotField. |
| Custom | `2` | Affiche les valeurs dans un format différent basé sur l'index de l'élément pivot dans le PivotField. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Définissez le format d'affichage des données pour afficher les valeurs comme différence par rapport à l'élément précédent
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Actualisez et calculez le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


