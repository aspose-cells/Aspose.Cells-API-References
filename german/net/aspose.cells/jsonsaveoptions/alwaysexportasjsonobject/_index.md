---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt an, ob Excel immer als JSON-Objekt exportiert wird, selbst wenn nur ein Arbeitsblatt in der Datei vorhanden ist"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn die Datei nur ein Arbeitsblatt enthält.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Beispielarbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Setzen Sie einige Beispieldaten im ersten Arbeitsblatt
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // JSON-Speicheroptionen konfigurieren
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // In JSON-Datei speichern
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Den gespeicherten JSON-Inhalt anzeigen
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


