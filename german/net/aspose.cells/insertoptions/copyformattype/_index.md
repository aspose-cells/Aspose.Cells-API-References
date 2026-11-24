---
title: "InsertOptions.CopyFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "InsertOptions-Eigenschaft."
type: docs
url: /de/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Werte und Formatierung für die Demonstration festlegen
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Erstelle InsertOptions und setze CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Zeile mit Formatierung aus dem Vorherigen einfügen
            worksheet.Cells.InsertRows(2, 1, options);

            // Ergebnis speichern
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


