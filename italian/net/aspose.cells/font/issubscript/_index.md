---
title: "Font.IsSubscript"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta un valore che indica se il carattere è in pedice"
type: docs
url: /it/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Ottiene o imposta un valore che indica se il carattere è pedice.

```csharp
public bool IsSubscript { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con testo in pedice
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Crea uno stile con testo in apice per confronto
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Applica gli stili alle celle
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Verifica e visualizza gli stili
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Salva la cartella di lavoro
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


