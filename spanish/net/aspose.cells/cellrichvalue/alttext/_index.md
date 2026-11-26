---
title: "CellRichValue.AltText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellRichValue. Obtiene el texto alternativo asociado a la imagen"
type: docs
url: /es/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Obtiene el texto alternativo asociado a la imagen.

```csharp
public virtual string AltText { get; set; }
```

### Ejemplos

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

### Ver también

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


