---
title: "Cells.ImportDataView"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa un DataView in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Importa un DataView in un foglio di lavoro.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataView | DataView | L'oggetto DataView da importare. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |

### Valore di ritorno

Numero totale di righe importate

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un DataTable di esempio
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Aggiungi dati di esempio
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // Crea DataView da DataTable
            DataView dataView = new DataView(table);

            // Importa DataView nel foglio di lavoro iniziando dalla riga 0, colonna 0
            cells.ImportDataView(dataView, 0, 0);

            // Salva la cartella di lavoro
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


