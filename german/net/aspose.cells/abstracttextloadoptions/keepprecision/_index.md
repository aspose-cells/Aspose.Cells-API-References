---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractTextLoadOptions-Eigenschaft. Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn seine Länge 15 beträgt"
type: docs
url: /de/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Gibt an, ob ein Zeichenkettenwert bei einer Länge von 15 nicht geparst wird.

```csharp
public bool KeepPrecision { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Erstellen Sie HTML-Ladeoptionen und setzen Sie KeepPrecision auf true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Lade die Arbeitsmappe mit den Optionen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrieren Sie, dass die Präzision beibehalten wird (z. B. numerische Werte mit vielen Dezimalstellen)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


