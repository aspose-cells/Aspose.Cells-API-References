---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLoadOptions-Eigenschaft. Gibt an, ob jedes Attribut des JsonObject-Objekts als ein Arbeitsblatt importiert wird, wenn alle Kindknoten Array-Knoten sind"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Gibt an, ob jedes Attribut des JsonObject-Objekts als ein Arbeitsblatt importiert wird, wenn alle Kindknoten Array-Knoten sind.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // JSON-Ladeoptionen mit aktiviertem MultipleWorksheets erstellen
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // JSON-Datei mit den angegebenen Optionen in die Arbeitsmappe laden
            Workbook workbook = new Workbook("example.json", options);
            
            // Daten aus dem ersten Arbeitsblatt abrufen
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Einige Beispielwerte aus dem geladenen JSON anzeigen
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### Siehe auch

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


