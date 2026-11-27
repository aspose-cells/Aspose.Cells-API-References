---
title: "TxtLoadOptions.Separator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Hämtar och anger teckenseparator för textfil"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Hämtar och anger teckenseparator för textfil.

```csharp
public char Separator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Skapa exempeldata och spara med anpassad separator
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // Läs in den sparade filen med samma separator
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Verifiera den inlästa datan
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


