---
title: "Classe PivotItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotItem. Représente un élément dans un rapport PivotField"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Représente un élément dans un rapport PivotField.

```csharp
public class PivotItem
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolète.**) Obtient l'index de l'élément pivot dans le champ de cache. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Indique si cet élément pivot est un élément de formule calculée. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Obtient et définit si le détail de cet élément pivot est masqué. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolète.**) Indique si cet élément pivot est un élément de formule calculée. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Obtient et définit si l'élément pivot est masqué. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolète.**) Obtient et définit si l'élément pivot masque le détail. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Indique si l'élément a été supprimé de la source de données. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Obtient le nom de l'élément pivot. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Spécifie l'index de cet élément parmi tous les PivotItems du champ. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsolète.**) Spécifie l'index de position dans les PivotItems sous le même nœud parent. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Obtient la valeur de l'élément pivot |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Obtient la valeur date/heure de l'élément pivot. Si la valeur est nulle, elle renverra DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Obtient la valeur double de l'élément pivot. Si la valeur est nulle ou n'est pas un nombre, elle renverra 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Obtient la formule de cet élément calculé. Fonctionne uniquement lorsque cet élément est un élément calculé. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Déplace l'élément vers le haut ou le bas dans le champ pivot |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsolète.**) Déplace l'élément vers le haut ou le bas |

## Champs

| Nom | Description |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Indice sentinelle de sélection de tous les éléments de page (0x7FFD, indice non valide) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accédez aux éléments pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Imprime le nom de l'élément pivot
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Définir les propriétés
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Imprime la valeur de l'élément pivot
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Utilisez les méthodes
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Enregistrez le classeur
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


