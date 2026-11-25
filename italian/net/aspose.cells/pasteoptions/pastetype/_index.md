---
title: "PasteOptions.PasteType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. Il tipo di incolla speciale"
type: docs
url: /it/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Il tipo di incolla speciale.

```csharp
public PasteType PasteType { get; set; }
```

### Esempi

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

            // Imposta il valore di origine
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Crea intervalli con nomi di tipo completamente qualificati
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Copia con PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Restituisci i risultati
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Vedi anche

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


