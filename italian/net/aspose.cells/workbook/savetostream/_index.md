---
title: "Workbook.SaveToStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Salva il file Excel in un oggetto MemoryStream come file Excel97-2003 xls e lo restituisce"
type: docs
url: /it/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Salva il file Excel in un oggetto MemoryStream come file xls Excel97-2003 e lo restituisce.

```csharp
public MemoryStream SaveToStream()
```

### Valore di ritorno

Oggetto MemoryStream che contiene un file Excel xls.

### Osservazioni

Questo metodo fornisce la stessa funzione del metodo Save e salva la cartella di lavoro solo come file Excel97-2003 xls. È principalmente per l'utilizzo da parte di client COM.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook start = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Salva la cartella di lavoro nello stream di memoria
            MemoryStream stream = start.SaveToStream();

            // Crea una nuova cartella di lavoro dallo stream
            Workbook workbook = new Workbook(stream);

            // Modifica la nuova cartella di lavoro
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


