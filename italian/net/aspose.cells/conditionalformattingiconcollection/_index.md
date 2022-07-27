---
title: ConditionalFormattingIconCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta una raccolta diConditionalFormattingIcon./conditionalformattingicon oggetti.
type: docs
weight: 1120
url: /it/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Rappresenta una raccolta di[`ConditionalFormattingIcon`](../conditionalformattingicon) oggetti.

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item) { get; } | Ottiene l'elemento ConditionalFormattingIcon in corrispondenza dell'indice specificato. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add)(ConditionalFormattingIcon) | Aggiunge[`ConditionalFormattingIcon`](../conditionalformattingicon) oggetto. |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add_1)(IconSetType, int) | Aggiunge[`ConditionalFormattingIcon`](../conditionalformattingicon) oggetto. |
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

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Ottieni la formattazione condizionale
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

//Aggiunge una formattazione condizionale vuota
int index = cformattings.Add();

//Ottieni la formattazione condizionale appena aggiunta
FormatConditionCollection fcs = cformattings[index];

//Imposta l'intervallo di formato condizionale.
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

//Imposta la condizione
 int idx = fcs.AddCondition(FormatConditionType.IconSet);
 
 FormatCondition cond = fcs[idx];
   
 //Imposta la condizione's type
 cond.IconSet.Type = IconSetType.ArrowsGray3;

//Aggiungi una condizione di set di icone personalizzata.
 ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
 
 cfIcon.Type = IconSetType.Arrows3;
 
 cfIcon.Index = 0;
 
 ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
 
  cfIcon1.Type = IconSetType.ArrowsGray3;
  
  cfIcon1.Index = 1;
  
  ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
  
  cfIcon2.Type = IconSetType.Boxes5;
  
  cfIcon2.Index = 2;

//Salvataggio del file Excel
workbook.Save("output.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Ottieni la formattazione condizionale
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Aggiunge una formattazione condizionale vuota
Dim index As Integer = cformattings.Add()

'Ottieni la formattazione condizionale appena aggiunta
Dim fcs As FormatConditionCollection = cformattings(index)

'Imposta l'intervallo di formato condizionale.
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

//Imposta la condizione
Dim idx As Integer =fcs.AddCondition(FormatConditionType.IconSet)

Dim cond As FormatCondition=fcs[idx]

//Imposta la condizione's type
cfIcon.Type = IconSetType.ArrowsGray3

'Aggiungi una condizione di set di icone personalizzate.
Dim cfIcon As ConditionalFormattingIcon = cond.IconSet.CfIcons[0]

cfIcon.Type = IconSetType.Arrows3

cfIcon.Index=0

Dim cfIcon1 As ConditionalFormattingIcon = cond.IconSet.CfIcons[1]

cfIcon1.Type = IconSetType.ArrowsGray3

cfIcon1.Index=1

Dim cfIcon2 As ConditionalFormattingIcon = cond.IconSet.CfIcons[2]

cfIcon2.Type = IconSetType.Boxes5

cfIcon2.Index=2

'Salvataggio del file Excel
workbook.Save("output.xls")
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [ConditionalFormattingIcon](../conditionalformattingicon)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
