---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Rimuove tutti gli oggetti di disegno in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Rimuove tutti gli oggetti di disegno in questo worksheet.

```csharp
public void RemoveAllDrawingObjects()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni oggetti di disegno al foglio di lavoro
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Salva prima di rimuovere gli oggetti
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Rimuovi tutti gli oggetti di disegno
            worksheet.RemoveAllDrawingObjects();
            
            // Salva dopo aver rimosso gli oggetti
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Elimina la cartella di lavoro
            workbook.Dispose();
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


