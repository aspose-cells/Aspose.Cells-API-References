---
title: "JsonSaveOptions.SkipEmptyRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om tomma rader ska hoppas över"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

Indikerar om tomma rader ska hoppas över.

```csharp
public bool SkipEmptyRows { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySkipEmptyRowsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Exempeldatat - lägg till några celler med värden och lämna några rader tomma
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Lämna rad 3 tom
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B4"].PutValue("Data4");

            // Konfigurera JSON-sparalternativ med SkipEmptyRows
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
            
            // Spara till JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


