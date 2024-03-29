---
title: RowCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Collecte les objets qui représentent les lignes individuelles dune feuille de calcul.
type: docs
weight: 5510
url: /fr/net/aspose.cells/rowcollection/
---
## RowCollection class

Collecte les objets qui représentent les lignes individuelles d'une feuille de calcul.

```csharp
public class RowCollection : IEnumerable
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count) { get; } | Obtient le nombre de lignes dans cette collection. |
| [Item](../../aspose.cells/rowcollection/item) { get; } | Obtient un objet par index de ligne donné. L'objet Row de l'index de ligne donné sera instancié s'il n'existe pas auparavant. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear)() | Effacer toutes les lignes et cellules. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator)() | Obtient un énumérateur qui parcourt cette collection |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex)(int) | Obtient l'objet ligne par la position dans la liste. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat)(int) | Supprimer la ligne à l'index spécifié |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

//Obtention de la référence de la première feuille de travail
Worksheet worksheet = workbook.Worksheets[0];
 // Récupère la première ligne
Row row = worksheet.Cells.Rows[0];

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

'Obtention de la référence de la première feuille de travail
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Obtenir la première ligne
Dim row as Row = worksheet.Cells.Rows(0)
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
