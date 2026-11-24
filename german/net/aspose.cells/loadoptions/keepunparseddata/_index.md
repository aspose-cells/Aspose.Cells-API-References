---
title: "LoadOptions.KeepUnparsedData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt an, ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden sollen, wenn sie aus einer Vorlagendatei geladen wird. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Hinweise

Für Szenarien, in denen der Benutzer nur einige Inhalte aus der Vorlagendatei lesen muss und die Arbeitsmappe nicht zurückspeichern muss, kann das Setzen dieser Eigenschaft auf false die Leistung verbessern, insbesondere in Kombination mit einer Art LoadFilter.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Erstelle LoadOptions und setze KeepUnparsedData auf false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Arbeitsmappe mit Optionen laden
            Workbook workbook = new Workbook("example.xlsx", options);

            // Greife auf das Arbeitsblatt zu und zeige, dass nicht geparste Daten nicht behalten werden
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


