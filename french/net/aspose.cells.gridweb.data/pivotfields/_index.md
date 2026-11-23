---
title: "Classe PivotFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotFields. Représente une collection de tous les objets PivotField dans un rapport de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Représente une collection de tous les objets [`PivotField`](../pivotfield/) dans un rapport de tableau croisé dynamique.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Obtient le nombre d'éléments contenus dans l'instance PivotFields |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Obtient une valeur indiquant si l'accès aux PivotFields est synchronisé (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Obtient un PivotField par index. (2 indexeurs) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Obtient l'objet parent pour l'objet spécifié. Lecture seule. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Obtient un objet pouvant être utilisé pour synchroniser l'accès aux PivotFields. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Copie l'intégralité du PivotField dans un tableau unidimensionnel compatible, en commençant à l'index spécifié du tableau cible |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Renvoie un IEnumerator pour les PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Obtient l'index du PivotField spécifié. |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridPivotFieldCollection à la place. Cette classe sera supprimée six mois après août 2014. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp

 [C#]

 //Obtient les PivotFields du PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Définit l'emplacement des PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Définit la fonction du champ de données
 field3.Function = PivotFieldFunction.Sum;

 //Modifie l'ordre des champs de ligne
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


