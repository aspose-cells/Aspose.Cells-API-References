---
title: "Style.IsDateTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se il formato numerico è un formato data"
type: docs
url: /it/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Indica se il formato numerico è un formato data.

```csharp
public bool IsDateTime { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Imposta un valore numerico
            cells["A1"].PutValue(1230);
            
            // Ottieni e modifica lo stile della cella
            Style style = cells["A1"].GetStyle();
            
            // Imposta al formato data (15 è il formato data predefinito)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Imposta un formato data personalizzato
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Applica lo stile modificato nuovamente alla cella
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


