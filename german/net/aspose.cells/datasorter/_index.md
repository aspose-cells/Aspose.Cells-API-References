---
title: DataSorter
second_title: Aspose.Cells für .NET-API-Referenz
description: Zusammenfassende Beschreibung für DataSorter.
type: docs
weight: 1300
url: /de/net/aspose.cells/datasorter/
---
## DataSorter class

Zusammenfassende Beschreibung für DataSorter.

```csharp
public class DataSorter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | Ermittelt und legt fest, ob beim Vergleichen von Zeichenfolgen zwischen Groß- und Kleinschreibung unterschieden wird. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | Gibt an, ob der Bereich Header hat. |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | Repräsentiert den ersten sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | Repräsentiert den zweiten sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | Repräsentiert den dritten sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | Ruft die Schlüsselliste des Datensortierers ab. |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | Stellt die Sortierreihenfolge des ersten Schlüssels dar. |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | Stellt die Sortierreihenfolge des zweiten Schlüssels dar. |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | Stellt die Sortierreihenfolge des dritten Schlüssels dar. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Gibt an, ob alles sortiert wird, was wie eine Zahl aussieht. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | Wahr bedeutet, dass die Sortierrichtung von links nach rechts ist. Falsch bedeutet, dass die Sortierrichtung von oben nach unten ist. Der Standardwert ist falsch. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [Clear](../../aspose.cells/datasorter/clear)() | Alle Einstellungen löschen. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Sortieren Sie die Daten im Bereich. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Sortieren Sie die Daten des Bereichs. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Sortiert die Daten des Bereichs. |

### Beispiele

```csharp

[C#]

//Instanziiere ein neues Workbook-Objekt.
Workbook workbook = new Workbook("Book1.xls");
//Datensortierer-Objekt der Arbeitsmappe abrufen.
DataSorter sorter = workbook.DataSorter;
//Legen Sie die erste Reihenfolge für das Datasorter-Objekt fest.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
//Den ersten Schlüssel definieren.
sorter.Key1 = 0;
//Legen Sie die zweite Reihenfolge für das Datasorter-Objekt fest.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
//Den zweiten Schlüssel definieren.
sorter.Key2 = 1;
//Einen Zellenbereich (Bereich) erstellen.
CellArea ca = new CellArea();
//Anfangszeilenindex angeben.
ca.StartRow = 0;
//Anfangsspaltenindex angeben.
ca.StartColumn = 0;
//Geben Sie den Index der letzten Zeile an.
ca.EndRow = 13;
//Letzten Spaltenindex angeben.
ca.EndColumn = 1;
//Daten im angegebenen Datenbereich sortieren (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
//Speichern Sie die Excel-Datei.
workbook.Save("outBook.xls");

[Visual Basic]

'Instanziieren Sie ein neues Workbook-Objekt.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Rufen Sie das Datasorter-Objekt der Arbeitsmappe ab.
Dim sorter As DataSorter = workbook.DataSorter
'Legen Sie die erste Reihenfolge für das Datasorter-Objekt fest
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Definieren Sie den ersten Schlüssel.
sorter.Key1 = 0
'Legen Sie die zweite Reihenfolge für das Datasorter-Objekt fest.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Definieren Sie den zweiten Schlüssel.
sorter.Key2 = 1
'Erstellen Sie einen Zellenbereich (Bereich).
Dim ca As CellArea = New CellArea
'Geben Sie den Startzeilenindex an.
ca.StartRow = 0
'Geben Sie den Startspaltenindex an.
ca.StartColumn = 0
'Geben Sie den letzten Zeilenindex an.
ca.EndRow = 13
'Geben Sie den letzten Spaltenindex an.
ca.EndColumn = 1
'Sortieren Sie die Daten im angegebenen Datenbereich (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Speichern Sie die Excel-Datei.
workbook.Save("outBook.xls")

```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
