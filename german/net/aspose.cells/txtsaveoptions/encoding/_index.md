---
title: "TxtSaveOptions.Encoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt die Standardkodierung zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Liest und setzt die Standardkodierung.

```csharp
public Encoding Encoding { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // Erstellen Sie TXT‑Speicheroptionen mit ASCII‑Kodierung
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Speichern Sie die Arbeitsmappe mit der angegebenen Kodierung
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


