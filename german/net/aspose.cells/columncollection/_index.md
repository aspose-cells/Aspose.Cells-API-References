---
title: ColumnCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Sammlung derObjekte die die einzelnen Spalteneinstellungen in einem Arbeitsblatt darstellen. Das Column-Objekt stellt nur die Einstellungen wie Spaltenbreite Stile usw. dar. für die ganze Spalte hat nichts damit zu tun dass es nicht leere Zellen Daten oder nicht in der entsprechenden Spalte gibt. Und die Anzahl dieser Sammlung stellt nur die Anzahl der darin instanziierten Spaltenobjekte dar Sammlung hat nichts damit zu tun dass es nicht leere Zellen Daten oder nicht im Arbeitsblatt gibt.
type: docs
weight: 1070
url: /de/net/aspose.cells/columncollection/
---
## ColumnCollection class

Sammlung derObjekte, die die einzelnen Spalten(einstellungen) in einem Arbeitsblatt darstellen. Das Column-Objekt stellt nur die Einstellungen wie Spaltenbreite, Stile usw. dar. für die ganze Spalte hat nichts damit zu tun, dass es nicht leere Zellen (Daten) oder nicht in der entsprechenden Spalte gibt. Und die "Anzahl" dieser Sammlung stellt nur die Anzahl der darin instanziierten Spaltenobjekte dar Sammlung, hat nichts damit zu tun, dass es nicht leere Zellen (Daten) oder nicht im Arbeitsblatt gibt.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | erhält a Objekt nach Spaltenindex. Das Spaltenobjekt des angegebenen Spaltenindex wird instanziiert, wenn es vorher nicht existiert. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Methoden

| Name | Beschreibung |
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
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Ruft die ab[`Column`](../column)Objekt durch die Position in der Liste. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

// Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.Worksheets[0];

// Neuen Stil zur Arbeitsmappe hinzufügen
Style style = workbook.CreateStyle();

// Setzen Sie die Hintergrundfarbe auf Blau
style.ForegroundColor = Color.Blue;

// Hintergrundmuster einstellen
style.Pattern = BackgroundType.Solid;

//Flag für neuen Stil
StyleFlag styleFlag = new StyleFlag();

//Alle Stile festlegen
styleFlag.All = true;

//Ändern Sie die Standardbreite der ersten zehn Spalten
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

//Spalte mit nicht standardmäßiger Formatierung abrufen
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    //Stil auf die ersten zehn Spalten anwenden
    column.ApplyStyle(style, styleFlag);
}

//Speichern der Excel-Datei
workbook.Save("book1.xls");

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()

'Abrufen der Referenz des ersten Arbeitsblatts
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Arbeitsmappe neuen Stil hinzufügen
Dim style As Style = workbook.CreateStyles()

'Setzen Sie die Hintergrundfarbe auf Blau
style.ForegroundColor = Color.Blue

'Einstellung Hintergrundmuster
style.Pattern = BackgroundType.Solid

'Flagge im neuen Stil
Dim styleFlag As New StyleFlag()

'Alle Stile einstellen
styleFlag.All = True

'Ändern Sie die Standardbreite der ersten zehn Spalten
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Rufen Sie die Spalte mit nicht standardmäßiger Formatierung ab
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Stil auf die ersten zehn Spalten anwenden
    column.ApplyStyle(style, styleFlag)
Next column

'Speichern der Excel-Datei
workbook.Save("book1.xls")

```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
