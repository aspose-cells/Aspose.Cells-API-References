---
title: ConditionalFormattingIconCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente une collection deConditionalFormattingIcon./conditionalformattingicon objets.
type: docs
weight: 1120
url: /fr/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Représente une collection de[`ConditionalFormattingIcon`](../conditionalformattingicon) objets.

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item) { get; } | Obtient l'élément ConditionalFormattingIcon à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add)(ConditionalFormattingIcon) | Ajoute[`ConditionalFormattingIcon`](../conditionalformattingicon) objet. |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add_1)(IconSetType, int) | Ajoute[`ConditionalFormattingIcon`](../conditionalformattingicon) objet. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Obtenir la mise en forme conditionnelle
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

//Ajoute une mise en forme conditionnelle vide
int index = cformattings.Add();

//Obtenir la mise en forme conditionnelle nouvellement ajoutée
FormatConditionCollection fcs = cformattings[index];

// Définit la plage de format conditionnel.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 0;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

ca = new CellArea();

ca.StartRow = 1;

ca.EndRow = 1;

ca.StartColumn = 1;

ca.EndColumn = 1;

fcs.AddArea(ca);

// Définit la condition
 int idx = fcs.AddCondition(FormatConditionType.IconSet);
 
 FormatCondition cond = fcs[idx];
   
 // Définit la condition's type
 cond.IconSet.Type = IconSetType.ArrowsGray3;

//Ajouter une condition de jeu d'icônes personnalisée.
 ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
 
 cfIcon.Type = IconSetType.Arrows3;
 
 cfIcon.Index = 0;
 
 ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
 
  cfIcon1.Type = IconSetType.ArrowsGray3;
  
  cfIcon1.Index = 1;
  
  ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
  
  cfIcon2.Type = IconSetType.Boxes5;
  
  cfIcon2.Index = 2;

//Enregistrement du fichier Excel
workbook.Save("output.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Obtenir la mise en forme conditionnelle
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Ajoute une mise en forme conditionnelle vide
Dim index As Integer = cformattings.Add()

'Obtenir la mise en forme conditionnelle nouvellement ajoutée
Dim fcs As FormatConditionCollection = cformattings(index)

'Définit la plage de format conditionnel.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 0

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

ca = New CellArea()

ca.StartRow = 1

ca.EndRow = 1

ca.StartColumn = 1

ca.EndColumn = 1

fcs.AddArea(ca)

// Définit la condition
Dim idx As Integer =fcs.AddCondition(FormatConditionType.IconSet)

Dim cond As FormatCondition=fcs[idx]

// Définit la condition's type
cfIcon.Type = IconSetType.ArrowsGray3

'Ajouter une condition de jeu d'icônes personnalisée.
Dim cfIcon As ConditionalFormattingIcon = cond.IconSet.CfIcons[0]

cfIcon.Type = IconSetType.Arrows3

cfIcon.Index=0

Dim cfIcon1 As ConditionalFormattingIcon = cond.IconSet.CfIcons[1]

cfIcon1.Type = IconSetType.ArrowsGray3

cfIcon1.Index=1

Dim cfIcon2 As ConditionalFormattingIcon = cond.IconSet.CfIcons[2]

cfIcon2.Type = IconSetType.Boxes5

cfIcon2.Index=2

'Enregistrement du fichier Excel
workbook.Save("output.xls")
```

### Voir également

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [ConditionalFormattingIcon](../conditionalformattingicon)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
