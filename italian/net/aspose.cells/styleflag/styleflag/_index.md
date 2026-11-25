---
title: "StyleFlag.StyleFlag"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore StyleFlag. Costruisce un oggetto con tutti i flag impostati a false"
type: docs
url: /it/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Costruisce un oggetto con tutti i flag impostati a false.

```csharp
public StyleFlag()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile in grassetto
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Applica lo stile alla riga 9 con il costruttore StyleFlag
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Inserisci un valore nella cella e verifica lo stile
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


