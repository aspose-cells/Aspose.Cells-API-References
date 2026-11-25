---
title: "Cells.DeleteBlankRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina tutte le righe vuote che non contengono dati o altri oggetti"
type: docs
url: /it/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Elimina tutte le righe vuote che non contengono alcun dato o altro oggetto.

```csharp
public void DeleteBlankRows()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati con righe vuote
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Elimina le righe vuote
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Elimina tutte le righe vuote che non contengono alcun dato o alcuni oggetti speciali come commenti visibili, tabelle pivot.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | DeleteOptions | Le opzioni di eliminazione dell'intervallo. |

### Osservazioni

Per le righe vuote che verranno eliminate, non è sufficiente che [`IsBlank`](../../row/isblank/) sia true, ma inoltre non deve esserci alcun commento visibile definito per qualsiasi cella in quelle righe, e nessuna tabella pivot il cui intervallo intersechi esse.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di test con righe vuote
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Crea opzioni di eliminazione
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Elimina le righe vuote
            sheet.Cells.DeleteBlankRows(options);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


