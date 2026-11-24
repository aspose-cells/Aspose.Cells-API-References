---
title: "Style.Custom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. Wenn das benutzerdefinierte Zahlenformat nicht gesetzt ist, wird beispielsweise das integrierte Zahlenformat zurückgegeben."
type: docs
url: /de/net/aspose.cells/style/custom/
---
## Style.Custom property

Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Style‑Objekts dar. Wenn das benutzerdefinierte Zahlenformat nicht gesetzt ist (z. B. das Zahlenformat ist eingebaut), wird \"\" zurückgegeben.

```csharp
public string Custom { get; set; }
```

### Hinweise

Die zurückgegebene benutzerdefinierte Zeichenfolge ist kulturunabhängig.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstellen und anwenden eines benutzerdefinierten Datumsformats
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Den formatierten Wert anzeigen
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


