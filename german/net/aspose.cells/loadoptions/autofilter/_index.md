---
title: "LoadOptions.AutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden"
type: docs
url: /de/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.

```csharp
public bool AutoFilter { get; set; }
```

### Hinweise

Manchmal, obwohl autofilter gesetzt ist, werden die entsprechenden Zeilen in der Datei nicht ausgeblendet. Jetzt funktioniert es nur für SpreadSheetML-Datei.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und AutoFilter aktivieren
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Arbeitsmappe laden mit aktiviertem AutoFilter
            Workbook workbook = new Workbook("example.xlsx", options);

            // Erste Arbeitsblatt öffnen und AutoFilter anwenden
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
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


