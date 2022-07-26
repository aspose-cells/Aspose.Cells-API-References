---
title: ColumnCollection
second_title: Aspose.Cells för .NET API-referens
description: Samling avobjekt som representerar de individuella kolumninställningerna i ett kalkylblad. Kolumnobjektet representerar endast inställningar som kolumnbredd stilar .etc. för hela kolumnen har ingenting att göra med det faktum att det finns icke-tomma cellerdata eller inte i motsvarande kolumn. Och Räknevärdet för denna samling representerar bara antalet kolumnobjekt som har instansierats i denna samling collection har ingenting att göra med det faktum att det finns icke-tomma cellerdata eller inte i kalkylbladet.
type: docs
weight: 1070
url: /sv/net/aspose.cells/columncollection/
---
## ColumnCollection class

Samling avobjekt som representerar de individuella kolumn(inställning)erna i ett kalkylblad. Kolumnobjektet representerar endast inställningar som kolumnbredd, stilar, .etc. för hela kolumnen har ingenting att göra med det faktum att det finns icke-tomma celler(data) eller inte i motsvarande kolumn. Och "Räknevärdet" för denna samling representerar bara antalet kolumnobjekt som har instansierats i denna samling collection, har ingenting att göra med det faktum att det finns icke-tomma celler(data) eller inte i kalkylbladet.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | Får en objekt för kolumn index. Kolumnobjektet för givet kolumnindex kommer att instansieras om det inte finns tidigare. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metoder

| namn | Beskrivning |
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
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Får[`Column`](../column)objekt efter positionen i listan. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();

//Hämta referensen till det första kalkylbladet
Worksheet worksheet = workbook.Worksheets[0];

//Lägg till ny stil i arbetsboken
Style style = workbook.CreateStyle();

//Ställer in bakgrundsfärgen till blå
style.ForegroundColor = Color.Blue;

//inställning av bakgrundsmönster
style.Pattern = BackgroundType.Solid;

//Ny stilflagga
StyleFlag styleFlag = new StyleFlag();

//Ange alla stilar
styleFlag.All = true;

//Ändra standardbredden för de första tio kolumnerna
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

//Hämta kolumnen med icke-standardformatering
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    //Tillämpa stil på de första tio kolumnerna
    column.ApplyStyle(style, styleFlag);
}

//Spara Excel-filen
workbook.Save("book1.xls");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()

'Få referensen till det första arbetsbladet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Lägg till ny stil i arbetsboken
Dim style As Style = workbook.CreateStyles()

'Ställer in bakgrundsfärgen till blå
style.ForegroundColor = Color.Blue

'inställning av bakgrundsmönster
style.Pattern = BackgroundType.Solid

'Ny stil flagga
Dim styleFlag As New StyleFlag()

'Ställ in alla stilar
styleFlag.All = True

'Ändra standardbredden för de första tio kolumnerna
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Hämta kolumnen med icke-standardformatering
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Tillämpa stil på de första tio kolumnerna
    column.ApplyStyle(style, styleFlag)
Next column

'Sparar Excel-filen
workbook.Save("book1.xls")

```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
