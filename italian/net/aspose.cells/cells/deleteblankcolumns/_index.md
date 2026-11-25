---
title: "Cells.DeleteBlankColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina tutte le colonne vuote che non contengono alcun dato"
type: docs
url: /it/net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Elimina tutte le colonne vuote che non contengono alcun dato.

```csharp
public void DeleteBlankColumns()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di test con colonne vuote
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
            worksheet.Cells["A2"].PutValue("Data A");
            worksheet.Cells["C2"].PutValue("Data C");
            
            // Elimina colonne vuote
            worksheet.Cells.DeleteBlankColumns();
            
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

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Elimina tutte le colonne vuote che non contengono alcun dato.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | DeleteOptions | Le opzioni di eliminazione dell'intervallo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati con colonne vuote
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["C2"].PutValue(3);

            Console.WriteLine("Before deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)

            // Configura le opzioni di eliminazione
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;

            // Elimina colonne vuote
            worksheet.Cells.DeleteBlankColumns(options);

            Console.WriteLine("After deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)

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


