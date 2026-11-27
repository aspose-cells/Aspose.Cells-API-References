---
title: "Style.Custom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Representerar den anpassade talformatsträngen för detta stilobjekt. Om den anpassade talformatet inte är angivet, t.ex. om talformatet är inbyggt, returneras det."
type: docs
url: /sv/net/aspose.cells/style/custom/
---
## Style.Custom property

Representerar den anpassade talformatsträngen för detta stilobjekt. Om det anpassade talformatet inte är angivet (till exempel om talformatet är inbyggt) returneras "".

```csharp
public string Custom { get; set; }
```

### Anmärkningar

Den returnerade anpassade strängen är kulturoberoende.

### Exempel

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

            // Skapa och tillämpa anpassat datumformat
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Visa det formaterade värdet
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Spara arbetsboken
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


