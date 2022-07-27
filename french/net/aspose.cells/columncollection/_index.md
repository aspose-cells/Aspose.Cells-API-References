---
title: ColumnCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Collecte desobjets qui représentent les colonnes individuelles paramètres dans une feuille de calcul. Lobjet Colonne représente uniquement les paramètres tels que la largeur de colonne les styles etc. pour toute la colonne na rien à voir avec le fait quil y ait des cellules données non vides ou non dans la colonne correspondante. Et le Count de cette collection ne représente que le nombre dobjets Column qui ont été instanciés dans cette collection na rien à voir avec le fait quil y ait des cellules données non vides ou non dans la feuille de calcul.
type: docs
weight: 1070
url: /fr/net/aspose.cells/columncollection/
---
## ColumnCollection class

Collecte desobjets qui représentent les colonnes individuelles (paramètres) dans une feuille de calcul. L'objet Colonne représente uniquement les paramètres tels que la largeur de colonne, les styles, etc. pour toute la colonne, n'a rien à voir avec le fait qu'il y ait des cellules (données) non vides ou non dans la colonne correspondante. Et le "Count" de cette collection ne représente que le nombre d'objets Column qui ont été instanciés dans cette collection, n'a rien à voir avec le fait qu'il y ait des cellules (données) non vides ou non dans la feuille de calcul.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | Obtient un objet par index de colonne. L'objet Colonne de l'index de colonne donné sera instancié s'il n'existe pas auparavant. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Obtient le[`Column`](../column)objet par la position dans la liste. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

//Obtention de la référence de la première feuille de travail
Worksheet worksheet = workbook.Worksheets[0];

//Ajouter un nouveau style au classeur
Style style = workbook.CreateStyle();

//Définition de la couleur d'arrière-plan sur Bleu
style.ForegroundColor = Color.Blue;

//définition du motif d'arrière-plan
style.Pattern = BackgroundType.Solid;

//Nouveau drapeau de style
StyleFlag styleFlag = new StyleFlag();

//Définir tous les styles
styleFlag.All = true;

//Modifier la largeur par défaut des dix premières colonnes
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

// Récupère la colonne avec une mise en forme non par défaut
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    //Appliquer le style aux dix premières colonnes
    column.ApplyStyle(style, styleFlag);
}

//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

'Obtention de la référence de la première feuille de travail
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Ajouter un nouveau style au classeur
Dim style As Style = workbook.CreateStyles()

'Définir la couleur d'arrière-plan sur Bleu
style.ForegroundColor = Color.Blue

'réglage du motif d'arrière-plan
style.Pattern = BackgroundType.Solid

'Nouveau drapeau de style
Dim styleFlag As New StyleFlag()

'Définir tous les styles
styleFlag.All = True

'Modifier la largeur par défaut des dix premières colonnes
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Obtenir la colonne avec une mise en forme non par défaut
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Appliquer le style aux dix premières colonnes
    column.ApplyStyle(style, styleFlag)
Next column

'Enregistrement du fichier Excel
workbook.Save("book1.xls")

```

### Voir également

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
