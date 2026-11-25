---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Crea un oggetto Range da un indirizzo dell'intervallo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Crea un oggetto [`Range`](../../range/) da un indirizzo dell'intervallo.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| address | String | L'indirizzo dell'intervallo. |
| sheetIndex | Int32 | L'indice del foglio. |

### Valore di ritorno

Un oggetto [`Range`](../../range/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo unione da stringhe di indirizzo
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Imposta il valore per l'intero intervallo di unione
            unionRange.Value = "Test";
            
            // Applica lo stile all'intervallo unione
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Salva la cartella di lavoro
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


