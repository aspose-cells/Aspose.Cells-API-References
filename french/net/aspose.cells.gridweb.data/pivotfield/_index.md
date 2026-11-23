---
title: "Classe PivotField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotField. Représente un champ dans un rapport PivotTable. L'objet PivotField est un membre de la collection PivotFields. NOTE : Cette classe est maintenant obsolète. Utilisez plutôt GridPivotField. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Représente un champ dans un rapport PivotTable. L'objet PivotField est un membre de la collection [`PivotFields`](../pivotfields/). NOTE : Cette classe est maintenant obsolète. Utilisez plutôt GridPivotField. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Le texte de l'étiquette du champ pivot affiché dans le rapport. Par défaut, affiche le nom. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Obtient les données du champ spécifié. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Représente la fonction utilisée pour résumer le champ PivotTable (uniquement les champs de données). La fonction par défaut est Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Obtient le nom. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Représente l'emplacement du champ dans le rapport PivotTable spécifié. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Représente la position du champ (premier, deuxième, troisième, etc.) parmi tous les champs de son orientation (Rows, Columns, Pages). Vous devez appeler la méthode get après l'appel de Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Représente l'ordre utilisé pour trier le champ PivotTable spécifié. |

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


