---
title: "TxtSaveOptions.Separator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Hämtar och anger tecknet Delimiter för textfilen"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Hämtar och anger tecknet avgränsare för textfilen.

```csharp
public char Separator { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Konfigurera TXT-sparalternativ med kommatecken som separator
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Spara arbetsboken som CSV med kommatecken som separator
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Visa det sparade filinnehållet
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


