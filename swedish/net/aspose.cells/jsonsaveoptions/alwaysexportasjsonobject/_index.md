---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om Excel alltid exporteras till JSON som objekt även om det bara finns ett kalkylblad i filen"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Anger om Excel alltid ska exporteras till JSON som objekt, även om det bara finns ett arbetsblad i filen.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ställ in lite exempeldata i det första kalkylbladet
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // Konfigurera JSON‑sparalternativ
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Spara till JSON‑fil
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Visa det sparade JSON‑innehållet
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


