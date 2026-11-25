---
title: "Style.ToJson"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Converte Style in dati struct JSON"
type: docs
url: /it/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Converti [`Style`](../) in dati struct JSON.

```csharp
public string ToJson()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea e applica uno stile alla cella B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Converti lo stile in JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Imposta la formula nella cella B6
            cells["B6"].Formula = "=A1";

            // Converti la cella in JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


