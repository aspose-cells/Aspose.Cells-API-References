---
title: "InsertOptions.CopyFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "InsertOptions egenskap."
type: docs
url: /sv/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Exempel

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

            // Ange värden och formatering för demonstration
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Skapa InsertOptions och ange CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Infoga rad med formatering från ovan
            worksheet.Cells.InsertRows(2, 1, options);

            // Spara resultatet
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Se även

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


