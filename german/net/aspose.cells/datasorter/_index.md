---
title: "Klasse DataSorter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataSorter Klasse. Zusammenfassende Beschreibung für DataSorter"
type: docs
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
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Liest und setzt, ob bei Zeichenkettenvergleich die Groß-/Kleinschreibung beachtet wird. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Gibt an, ob der Bereich Überschriften enthält. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Gibt den Index der zuerst sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Gibt den Index der zweitens sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Gibt den Index der drittens sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Liefert die Schlüsselliste des DataSorters. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Gibt die Sortierreihenfolge des ersten Schlüssels an. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Gibt die Sortierreihenfolge des zweiten Schlüssels an. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Gibt die Sortierreihenfolge des dritten Schlüssels an. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True bedeutet, dass die Sortierrichtung von links nach rechts verläuft. False bedeutet, dass die Sortierrichtung von oben nach unten verläuft. Der Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Fügt Farbsortierschlüssel hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Alle Einstellungen zurücksetzen. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Sortiere die Daten im Bereich. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Sortiere die Daten des Bereichs. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Sortiert die Daten des Bereichs. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Instanziiere ein neues Workbook-Objekt
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Hole das Workbook DataSorter-Objekt
            DataSorter sorter = workbook.DataSorter;

            // Setze die erste Reihenfolge für das DataSorter-Objekt.
            sorter.Order1 = SortOrder.Descending;
            // Definiere den ersten Schlüssel.
            sorter.Key1 = 0;

            // Setze die zweite Reihenfolge für das DataSorter-Objekt.
            sorter.Order2 = SortOrder.Ascending;
            // Definiere den zweiten Schlüssel.
            sorter.Key2 = 1;

            // Erstelle einen Zellenbereich (Bereich)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Sortiere Daten im angegebenen Datenbereich (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Speichere die Excel-Datei
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


