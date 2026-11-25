---
title: "CellRichValue.AltText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellRichValue. Ottiene il testo alternativo associato all'immagine"
type: docs
url: /it/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Ottiene il testo alternativo associato all'immagine.

```csharp
public virtual string AltText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyAltTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["C4"];
            
            cell.GetRichValue().AltText = "test alt text";
            
            Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
        }
    }
}
```

### Vedi anche

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


