---
title: "Gränssnitt ICellsDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ICellsDataTable-gränssnitt. Representerar en datatabell"
type: docs
url: /sv/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Representerar datatabell.

```csharp
public interface ICellsDataTable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Hämtar kolumnens namn. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Hämtar antalet poster. -1 för okänt antal poster. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Hämtar data som lagras i kolumnen som specificerats med index. (2 indexerare) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Flytta markören till början av detta objekt, precis före den första raden. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Flyttar markören ner en rad från dess nuvarande position. |

### Exempel

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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


