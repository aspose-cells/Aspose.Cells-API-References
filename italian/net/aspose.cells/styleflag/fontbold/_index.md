---
title: "StyleFlag.FontBold"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione del grassetto del carattere verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

L'impostazione di grassetto del carattere sarà applicata.

```csharp
public bool FontBold { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile in grassetto
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Applica lo stile in grassetto alla riga 2 con StyleFlag solo per FontBold
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Inserisci valore nella cella per dimostrare lo stile
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


