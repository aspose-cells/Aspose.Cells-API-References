---
title: "Font.Charset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Rappresenta il set di caratteri"
type: docs
url: /it/net/aspose.cells/font/charset/
---
## Font.Charset property

Rappresenta il set di caratteri.

```csharp
public int Charset { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con proprietà di carattere specifiche, incluso il set di caratteri
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Crea un altro stile con un set di caratteri diverso
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Applica il secondo stile a un'altra cella
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Salva la cartella di lavoro
            workbook.Save("FontCharsetDemo.xlsx");

            // Verifica le proprietà del set di caratteri
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


