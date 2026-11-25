---
title: "Cell.HtmlString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell proprietà. Ottiene e imposta la stringa html che contiene dati e alcuni formati in questa cella"
type: docs
url: /it/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Restituisce e imposta la stringa HTML che contiene dati e alcuni formati in questa cella.

```csharp
public string HtmlString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Crea un'istanza di cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di celle
            Cells cells = worksheet.Cells;
            
            // Imposta la stringa HTML con formattazione nella cella A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Salva la cartella di lavoro
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


