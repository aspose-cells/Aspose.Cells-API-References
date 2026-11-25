---
title: "Interfaccia ICellsDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.ICellsDataTable. Rappresenta una tabella dati"
type: docs
url: /it/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Rappresenta la tabella dei dati.

```csharp
public interface ICellsDataTable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Ottiene il nome delle colonne. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Ottiene il conteggio dei record. -1 per conteggio dei record sconosciuto. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Ottiene i dati memorizzati nella colonna specificata per indice. (2 indicizzatori) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Sposta il cursore all'inizio di questo oggetto, appena prima della prima riga. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Sposta il cursore verso il basso di una riga dalla sua posizione attuale. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


