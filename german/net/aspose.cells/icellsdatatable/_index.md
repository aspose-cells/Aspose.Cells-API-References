---
title: "Schnittstelle ICellsDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ICellsDataTable‑Schnittstelle. Stellt eine Datentabelle dar"
type: docs
url: /de/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Stellt eine Datentabelle dar.

```csharp
public interface ICellsDataTable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Liest den Namen der Spalten. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Liest die Anzahl der Datensätze. -1 für unbekannte Datensatzanzahl. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Liest die in der durch den Index angegebenen Spalte gespeicherten Daten. (2 Indexer) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Bewege den Cursor an den Anfang dieses Objekts, direkt vor die erste Zeile. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Bewegt den Cursor eine Zeile nach unten von seiner aktuellen Position. |

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


