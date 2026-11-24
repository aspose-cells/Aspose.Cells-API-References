---
title: "Font.IsSubscript"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Schrift tiefgestellt ist"
type: docs
url: /de/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift tiefgestellt ist.

```csharp
public bool IsSubscript { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil mit tiefgestelltem Text
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Erstellen Sie einen Stil mit hochgestelltem Text zum Vergleich
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Stile auf Zellen anwenden
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Überprüfen und zeigen Sie die Stile an
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Speichere die Arbeitsmappe
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


