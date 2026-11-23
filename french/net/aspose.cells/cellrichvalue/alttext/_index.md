---
title: "CellRichValue.AltText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CellRichValue propriété. Obtient le texte alternatif associé à l'image"
type: docs
url: /fr/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Obtient le texte alternatif associé à l'image.

```csharp
public virtual string AltText { get; set; }
```

### Exemples

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

### Voir aussi

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


