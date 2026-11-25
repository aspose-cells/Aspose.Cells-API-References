---
title: "DeleteOptions.UpdateReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteOptions. Indica se aggiornare i riferimenti in altri fogli di lavoro"
type: docs
url: /it/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Indica se aggiornare i riferimenti in altri fogli di lavoro.

```csharp
public bool UpdateReference { get; set; }
```

### Osservazioni

A partire dalla versione 26.7 impostiamo il valore predefinito di questa proprietà a true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formule
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Crea opzioni di eliminazione con UpdateReference impostato su vero
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Elimina la colonna A che è referenziata nelle formule
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


