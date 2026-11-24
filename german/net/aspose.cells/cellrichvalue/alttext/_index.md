---
title: "CellRichValue.AltText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellRichValue-Eigenschaft. Ruft den mit dem Bild verbundenen Alternativtext ab"
type: docs
url: /de/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Liest den alternativen Text, der mit dem Bild verknüpft ist.

```csharp
public virtual string AltText { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


