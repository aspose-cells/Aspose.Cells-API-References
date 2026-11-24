---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt den Typ des Exports von Hyperlinks zu JSON an"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Stellt den Typ des Exports von Hyperlinks nach JSON dar.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Hinweise

Der Standardwert ist DisplayString;

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen Hyperlink zu Zelle A1 hinzu
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Exportoptionen für JSON festlegen
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Arbeitsmappe als JSON speichern
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Überprüfen, ob die Ausgabe den Hyperlink enthält
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### Siehe auch

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


