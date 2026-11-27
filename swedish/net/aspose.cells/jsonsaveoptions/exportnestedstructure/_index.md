---
title: "JsonSaveOptions.ExportNestedStructure"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions‑egenskap. Exporteras som en förälder‑barn‑hierarki i Json‑struktur"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

Exporterad som parent-child hierarki Json-struktur.

```csharp
public bool ExportNestedStructure { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportNestedStructureDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med nästlad data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en nästlad datastruktur
            worksheet.Cells["A1"].PutValue("Parent");
            worksheet.Cells["B1"].PutValue("Child");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Fruits");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Vegetables");
            worksheet.Cells["B4"].PutValue("Carrot");

            // Konfigurera JSON‑sparalternativ med ExportNestedStructure
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            saveOptions.AlwaysExportAsJsonObject = true;

            // Spara med nästlad struktur
            string outputPath = "output_nested.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


