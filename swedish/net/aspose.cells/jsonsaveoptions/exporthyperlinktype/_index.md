---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Representerar typen av export av hyperlänk till json"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Representerar typen av export av hyperlänk till JSON.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Anmärkningar

Standardvärdet är DisplayString;

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en hyperlänk till cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Ställ in exportalternativ för JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Spara arbetsbok till JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Verifiera att utdata innehåller hyperlänken
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### Se även

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


