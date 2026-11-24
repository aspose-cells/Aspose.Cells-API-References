---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob überlaufender Text ausgeblendet wird, wenn das Zellenformat auf Zeilenumbruch eingestellt ist. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false.

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext in Zelle A1 festlegen
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Stil mit Textumbruch erstellen und anwenden
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Die Zellsammlung abrufen und Stil anwenden
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Spaltenbreite festlegen, damit der Text umbricht
            cells.SetColumnWidth(0, 10);
            
            // HTML-Speicheroptionen erstellen und HideOverflowWrappedText festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Arbeitsmappe mit HTML‑Optionen speichern
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


