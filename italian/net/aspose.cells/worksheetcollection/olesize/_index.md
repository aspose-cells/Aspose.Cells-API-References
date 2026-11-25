---
title: "WorksheetCollection.OleSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Ottiene e imposta la dimensione visualizzata quando il file Workbook è usato come oggetto OLE"
type: docs
url: /it/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Ottiene e imposta la dimensione visualizzata quando il file Workbook è usato come oggetto Ole.

```csharp
public object OleSize { get; set; }
```

### Osservazioni

Null indica nessuna impostazione di dimensione OLE.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la dimensione OLE per la collezione di fogli di lavoro
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Accedi e visualizza le proprietà della dimensione OLE
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Salva la cartella di lavoro
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


