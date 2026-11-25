---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteBlankOptions. Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola il foglio di lavoro con dati includendo stringhe vuote
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Configura DeleteBlankOptions con EmptyStringAsBlank impostato su true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Elimina le righe contenenti stringhe vuote (trattate come vuote)
            worksheet.Cells.DeleteBlankRows(options);

            // Salva il risultato
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


