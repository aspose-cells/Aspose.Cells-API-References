---
title: "Klasse ColumnCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ColumnCollection class. Sammlung der Column-Objekte, die die einzelnen Spalteneinstellungen in einem Arbeitsblatt darstellen. Das Column-Objekt stellt nur Einstellungen wie Spaltenbreite, Stile usw. für die gesamte Spalte dar und hat nichts damit zu tun, ob in der entsprechenden Spalte nicht-leere Zellen/Daten vorhanden sind oder nicht. Und die Count‑Eigenschaft dieser Sammlung gibt nur die Anzahl der Column‑Objekte an, die in dieser Sammlung instanziiert wurden; sie hat ebenfalls nichts damit zu tun, ob im Arbeitsblatt nicht-leere Zellen/Daten vorhanden sind."
type: docs
url: /de/net/aspose.cells/columncollection/
---
## ColumnCollection class

Sammlung der [`Column`](../column/)-Objekte, die die einzelnen Spalten(einstellungen) in einem Arbeitsblatt darstellen. Das Column-Objekt stellt nur Einstellungen wie Spaltenbreite, Stile usw. für die gesamte Spalte dar und hat nichts damit zu tun, ob in der entsprechenden Spalte nicht‑leere Zellen (Daten) vorhanden sind oder nicht. Und die "Count"‑Eigenschaft dieser Sammlung gibt nur die Anzahl der Column‑Objekte an, die in dieser Sammlung instanziiert wurden; sie hat nichts damit zu tun, ob im Arbeitsblatt nicht‑leere Zellen (Daten) vorhanden sind.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Ruft ein [`Column`](../column/)-Objekt anhand des Spaltenindex ab. Das Column-Objekt des angegebenen Spaltenindex wird instanziiert, falls es vorher nicht existiert. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsolete.**) Ruft das Spaltenobjekt anhand des Index ab. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Ruft das [`Column`](../column/)-Objekt anhand seiner Position in der Liste ab. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Neuen Stil zur Arbeitsmappe hinzufügen
            Style style = workbook.CreateStyle();

            // Setzt die Hintergrundfarbe auf Blau
            style.ForegroundColor = Color.Blue;

            // Setzt das Hintergrundmuster
            style.Pattern = BackgroundType.Solid;

            // Neues Stil-Flag
            StyleFlag styleFlag = new StyleFlag();

            // Alle Stile festlegen
            styleFlag.All = true;

            // Standardbreite der ersten zehn Spalten ändern
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Spalte mit nicht‑standardmäßiger Formatierung abrufen
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Stil auf die ersten zehn Spalten anwenden
                column.ApplyStyle(style, styleFlag);
            }

            // Die Excel-Datei speichern
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


