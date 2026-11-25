---
title: "Enum ProtectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ProtectionType enum. Rappresenta il tipo di protezione del workbook/worksheet"
type: docs
url: /it/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Rappresenta il tipo di protezione della cartella di lavoro/foglio di lavoro.

```csharp
public enum ProtectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| All | `0` | Rappresenta la protezione totale. |
| Contents | `1` | Rappresenta la protezione del contenuto, usata nella protezione del foglio di lavoro. |
| Objects | `2` | Rappresenta la protezione degli oggetti, usata nella protezione del foglio di lavoro. |
| Scenarios | `3` | Rappresenta la protezione degli scenari, usata nella protezione del foglio di lavoro. |
| Structure | `4` | Rappresenta la protezione della struttura, usata nella protezione del workbook. |
| Windows | `5` | Rappresenta la protezione della finestra, usata nella protezione del workbook. |
| None | `6` | Rappresenta nessuna protezione. Solo per la proprietà Reading. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con tutti i tipi di protezione
            worksheet.Protect(ProtectionType.All);
            
            // Dimostra l'accesso alle proprietà di protezione
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Rimuovi la protezione dal foglio di lavoro
            worksheet.Unprotect();
            
            // Proteggi con tipi di protezione specifici
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


