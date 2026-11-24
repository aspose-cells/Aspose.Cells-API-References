---
title: "JsonSaveOptions.ExportAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Exportiert den Zeichenwert der Zellen nach JSON"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Exportiert den Zeichenkettenwert der Zellen nach JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Beispieldaten mit numerischen Werten erstellen
            cells["A1"].PutValue("Age");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue(30);
            cells["B2"].PutValue(95.5);

            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
            Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


