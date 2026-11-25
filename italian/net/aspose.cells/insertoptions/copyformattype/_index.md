---
title: "InsertOptions.CopyFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà InsertOptions."
type: docs
url: /it/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Esempi

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

            // Imposta valori e formattazione per la dimostrazione
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Crea InsertOptions e imposta CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Inserisci una riga con la formattazione sopra
            worksheet.Cells.InsertRows(2, 1, options);

            // Salva il risultato
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


