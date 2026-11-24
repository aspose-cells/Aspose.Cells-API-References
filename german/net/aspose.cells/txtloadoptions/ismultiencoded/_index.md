---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. True bedeutet, dass die Datei mehrere Codierungen enthält"
type: docs
url: /de/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True bedeutet, dass die Datei mehrere Kodierungen enthält.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Erstelle Text-Ladeoptionen
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Setze IsMultiEncoded auf true, um mehrere Codierungen zu verarbeiten
            options.IsMultiEncoded = true;
            
            // Lade die Arbeitsmappe mit den Optionen
            Workbook workbook = new Workbook("example.csv", options);
            
            // Zeige Beispielwerte aus der geladenen Datei an
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


