---
title: "Style.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-konstruktor. Initierar en ny instans av Style-klassen"
type: docs
url: /sv/net/aspose.cells/style/style/
---
## Style constructor

Initierar en ny instans av [`Style`](../)-klassen.

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Anmärkningar

OBS: Den här konstruktorn är nu föråldrad. Använd istället metoden CellsFactory.CreateStyle(). Den här egenskapen kommer att tas bort 6 månader senare sedan oktober 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med hjälp av konstruktorn
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


