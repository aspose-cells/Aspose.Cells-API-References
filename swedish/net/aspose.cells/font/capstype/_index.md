---
title: "Font.CapsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar och anger textens versaltyp"
type: docs
url: /sv/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Hämtar och anger textens versaltyp.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Anmärkningar

Endast för teckensnitten i Shapes eller Charts. OBS: Denna medlem är nu föråldrad. Använd istället [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/) egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


