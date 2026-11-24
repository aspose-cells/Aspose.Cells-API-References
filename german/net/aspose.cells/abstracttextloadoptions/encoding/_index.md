---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractTextLoadOptions-Eigenschaft. Gibt die Standardkodierung zurück und legt sie fest. Gilt nur für CSV-Dateien"
type: docs
url: /de/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Liest und setzt die Standardkodierung. Gilt nur für CSV-Dateien.

```csharp
public Encoding Encoding { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Erstelle Beispieldaten im CSV-Format mit ASCII-Kodierung
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // Lade Arbeitsmappe mit angegebener ASCII-Kodierung
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Zeige geladene Daten an
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Füge etwas Unicode-Text hinzu
            cells[2, 0].PutValue("日本語のテキスト");
            
            // Speichere mit UTF-8-Kodierung
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // Zeige die ersten Bytes, um den UTF-8-BOM zu zeigen
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


