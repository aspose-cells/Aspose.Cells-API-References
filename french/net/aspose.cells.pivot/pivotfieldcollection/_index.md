---
title: "Classe PivotFieldCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotFieldCollection. Représente une collection de tous les objets PivotField dans les différentes régions du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/
---
## PivotFieldCollection class

Représente une collection de tous les objets PivotField dans les différentes régions du tableau croisé dynamique.

```csharp
public class PivotFieldCollection : CollectionBase<PivotField>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotfieldcollection/item/) { get; } | Obtient l'objet PivotField à l'index spécifique. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Type](../../aspose.cells.pivot/pivotfieldcollection/type/) { get; } | Obtient le type des PivotFields. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfieldcollection/add/)(PivotField) | Ajoute un objet PivotField au type spécifique PivotFields. |
| [AddByBaseIndex](../../aspose.cells.pivot/pivotfieldcollection/addbybaseindex/)(int) | Ajoute un objet PivotField au type spécifique PivotFields. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField, IComparer&lt;PivotField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotField, IComparer&lt;PivotField&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivotfieldcollection/clear/#clear)() | efface tous les champs de PivotFieldCollection (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotField) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotField[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotField&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotField&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int, int) |  |
| [Insert](../../aspose.cells.pivot/pivotfieldcollection/insert/)(int, PivotField) | Insère un champ pivot à un index spécifique. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int, int) |  |
| [Move](../../aspose.cells.pivot/pivotfieldcollection/move/)(int, int) | Déplace le PivotField de la position actuelle vers la position de destination |
| [Remove](../../aspose.cells.pivot/pivotfieldcollection/remove/)(PivotField) | Supprime le champ de la région actuelle. |
| [RemoveAt](../../aspose.cells.pivot/pivotfieldcollection/removeat/#removeat)(int) | Supprime le champ par l'index. Seulement pour les régions filtre, ligne, colonne, données. (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionDemo
    {
        public static void PivotFieldCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Accédez à la collection RowFields
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Affiche le nombre de champs de ligne
            Console.WriteLine("Row Fields Count: " + rowFields.Count);

            // Accédez au premier champ de ligne et affichez son nom
            PivotField firstRowField = rowFields[0];
            Console.WriteLine("First Row Field Name: " + firstRowField.Name);

            // Ajoutez un nouveau champ par indice de base
            int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the "Year" field to the row area
            Console.WriteLine("New Field Index: " + newFieldIndex);

            // Effacez tous les champs de la collection RowFields
            rowFields.Clear();
            Console.WriteLine("Row Fields Count after Clear: " + rowFields.Count);

            // Enregistrez le classeur
            workbook.Save("PivotFieldCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotField](../pivotfield/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


