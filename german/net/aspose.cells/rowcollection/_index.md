---
title: RowCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Sammelt die Objekte die die einzelnen Zeilen in einem Arbeitsblatt darstellen.
type: docs
weight: 5510
url: /de/net/aspose.cells/rowcollection/
---
## RowCollection class

Sammelt die Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen.

```csharp
public class RowCollection : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count) { get; } | Ruft die Anzahl der Zeilen in dieser Sammlung ab. |
| [Item](../../aspose.cells/rowcollection/item) { get; } | erhält a Objekt nach gegebenem Zeilenindex. Das Zeilenobjekt des angegebenen Zeilenindex wird instanziiert, wenn es vorher nicht existiert. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear)() | Alle Zeilen und Zellen löschen. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator)() | Ruft einen Enumerator ab, der diese Sammlung durchläuft |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex)(int) | Ruft das Zeilenobjekt nach Position in der Liste ab. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat)(int) | Entfernen Sie die Zeile am angegebenen Index |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

// Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.Worksheets[0];
 //Erste Zeile abrufen
Row row = worksheet.Cells.Rows[0];

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()

'Abrufen der Referenz des ersten Arbeitsblatts
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Erste Reihe erhalten
Dim row as Row = worksheet.Cells.Rows(0)
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
