---
title: "Font.Charset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Stellt den Zeichensatz dar"
type: docs
url: /de/net/aspose.cells/font/charset/
---
## Font.Charset property

Stellt den Zeichensatz dar.

```csharp
public int Charset { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil mit spezifischen Schriftarteigenschaften einschließlich Zeichensatz
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Erstellen Sie einen weiteren Stil mit anderem Zeichensatz
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Wende den zweiten Stil auf eine andere Zelle an
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Speichere die Arbeitsmappe
            workbook.Save("FontCharsetDemo.xlsx");

            // Überprüfen Sie die Zeichensatz‑Eigenschaften
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


