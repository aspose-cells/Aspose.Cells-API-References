---
title: "Cells.ImportDataRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa una DataRow nel file Excel"
type: docs
url: /it/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Importa un DataRow nel file Excel.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataRow | DataRow | Oggetto DataRow. |
| riga | Int32 | Indice della riga. |
| firstColumn | Int32 | Indice della prima colonna. |

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un DataTable di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Aggiungi dati di esempio
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Importa la prima riga da DataTable al foglio di lavoro iniziando dalla riga 0, colonna 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Salva la cartella di lavoro
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


