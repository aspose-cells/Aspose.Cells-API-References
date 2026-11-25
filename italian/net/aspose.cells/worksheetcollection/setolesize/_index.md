---
title: "WorksheetCollection.SetOleSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Imposta la dimensione visualizzata quando il file Workbook è usato come oggetto Ole"
type: docs
url: /it/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Imposta la dimensione visualizzata quando il file Workbook è usato come oggetto Ole.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| endRow | Int32 | Indice della riga finale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endColumn | Int32 | Indice della colonna finale. |

### Osservazioni

Questo metodo è generalmente usato per regolare la dimensione di visualizzazione in file ppt o file doc.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la dimensione OLE per i fogli di lavoro
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica la dimensione OLE
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


