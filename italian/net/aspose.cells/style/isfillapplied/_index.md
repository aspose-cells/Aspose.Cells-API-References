---
title: "Style.IsFillApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione di riempimento deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Indica se la formattazione di riempimento deve essere applicata.

```csharp
public bool IsFillApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile
            Style style = workbook.CreateStyle();
            
            // Inizialmente, IsFillApplied dovrebbe essere false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Applica le impostazioni di riempimento
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Dopo aver impostato le proprietà di riempimento, IsFillApplied dovrebbe essere true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Applica lo stile a una cella
            worksheet.Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


