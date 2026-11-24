---
title: "Klasse RowCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.RowCollection-Klasse. Sammelt die Row-Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen"
type: docs
url: /de/net/aspose.cells/rowcollection/
---
## RowCollection class

Sammelt die [`Row`](../row/) Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen.

```csharp
public class RowCollection : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Ermittelt die Anzahl der Zeilen in dieser Sammlung. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Ermittelt ein [`Row`](../row/) Objekt anhand des angegebenen Zeilenindex. Das Row-Objekt des angegebenen Zeilenindex wird instanziiert, falls es vorher nicht existiert. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Löschen Sie alle Zeilen und Zellen. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Ermittelt einen Enumerator, der die Zeilen dieser Sammlung durchläuft |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Ermittelt einen Enumerator, der die Zeilen dieser Sammlung durchläuft |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Ermittelt das Zeilenobjekt anhand seiner Position in der Liste. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Entfernen Sie das Zeilenelement am angegebenen Index (Position) in dieser Sammlung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Rufen Sie die Rows-Sammlung ab
            RowCollection rows = worksheet.Cells.Rows;

            // Rufen Sie die Anzahl der Zeilen in der Sammlung ab
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Rufen Sie die erste Zeile ab
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Iterieren Sie durch die Zeilen mit GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Rufen Sie eine Zeile anhand des Index ab
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Löschen Sie alle Zeilen und Zellen
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Speichere die Arbeitsmappe
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


