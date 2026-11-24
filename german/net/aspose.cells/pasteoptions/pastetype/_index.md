---
title: "PasteOptions.PasteType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Der Spezial‑Einfügetyp"
type: docs
url: /de/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Der Spezial‑Einfügetyp.

```csharp
public PasteType PasteType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Quellwert festlegen
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Bereiche mit vollqualifizierten Typnamen erstellen
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Kopieren mit PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Ergebnisse ausgeben
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Siehe auch

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


