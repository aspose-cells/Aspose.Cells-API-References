---
title: ColumnCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Raccolta dioggetti che rappresentano le singole colonne impostazioni in un foglio di lavoro. Loggetto Colonna rappresenta solo le impostazioni come la larghezza della colonna gli stili ecc. per lintera colonna non ha nulla a che fare con il fatto che ci sono celle dati non vuote o non nella colonna corrispondente. E il Count di questa raccolta rappresenta solo il conteggio oggetti Colonna che sono stati istanziati in questo raccolta non ha nulla a che fare con il fatto che ci sono celle dati non vuote o meno nel foglio di lavoro.
type: docs
weight: 1070
url: /it/net/aspose.cells/columncollection/
---
## ColumnCollection class

Raccolta dioggetti che rappresentano le singole colonne (impostazioni) in un foglio di lavoro. L'oggetto Colonna rappresenta solo le impostazioni come la larghezza della colonna, gli stili, ecc. per l'intera colonna, non ha nulla a che fare con il fatto che ci sono celle (dati) non vuote o non nella colonna corrispondente. E il "Count" di questa raccolta rappresenta solo il conteggio oggetti Colonna che sono stati istanziati in questo raccolta, non ha nulla a che fare con il fatto che ci sono celle (dati) non vuote o meno nel foglio di lavoro.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | Ottiene a oggetto per indice di colonna. L'oggetto Colonna di un dato indice di colonna verrà istanziato se non esisteva prima. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metodi

| Nome | Descrizione |
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
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Ottiene il[`Column`](../column)oggetto dalla posizione nell'elenco. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

//Ottenere il riferimento del primo foglio di lavoro
Worksheet worksheet = workbook.Worksheets[0];

//Aggiungi un nuovo stile alla cartella di lavoro
Style style = workbook.CreateStyle();

//Impostazione del colore di sfondo su Blu
style.ForegroundColor = Color.Blue;

//impostazione del motivo di sfondo
style.Pattern = BackgroundType.Solid;

//Nuovo stile bandiera
StyleFlag styleFlag = new StyleFlag();

//Imposta tutti gli stili
styleFlag.All = true;

//Modifica la larghezza predefinita delle prime dieci colonne
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

//Ottieni la colonna con una formattazione non predefinita
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    //Applica lo stile alle prime dieci colonne
    column.ApplyStyle(style, styleFlag);
}

//Salvataggio del file Excel
workbook.Save("book1.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

'Ottenere il riferimento del primo foglio di lavoro
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Aggiungi un nuovo stile alla cartella di lavoro
Dim style As Style = workbook.CreateStyles()

'Impostare il colore di sfondo su Blu
style.ForegroundColor = Color.Blue

'impostazione del motivo di sfondo
style.Pattern = BackgroundType.Solid

'Nuovo stile bandiera
Dim styleFlag As New StyleFlag()

'Imposta tutti gli stili
styleFlag.All = True

'Modifica la larghezza predefinita delle prime dieci colonne
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Ottieni la colonna con una formattazione non predefinita
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Applica lo stile alle prime dieci colonne
    column.ApplyStyle(style, styleFlag)
Next column

'Salvataggio del file Excel
workbook.Save("book1.xls")

```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
