---
title: "TxtSaveOptions.SeparatorString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt einen Zeichenkettenwert als Trennzeichen zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

Liest und setzt einen Zeichenkettenwert als Trennzeichen.

```csharp
public string SeparatorString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Testdaten hinzu.
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue(2);

            // Mit Leerzeichen als Trennzeichen speichern
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = " ";
            workbook.Save("output_space.txt", saveOptions);

            // Mit Pipe-Trennzeichen speichern
            saveOptions.SeparatorString = "|";
            workbook.Save("output_pipe.txt", saveOptions);

            // Laden Sie die durch Leerzeichen getrennte Datei zum Überprüfen
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = " ";
            Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;

            Console.WriteLine("Space-separated values:");
            Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
            Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
            Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


